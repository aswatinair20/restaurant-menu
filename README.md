# restaurant-menu

<!DOCTYPE html>
<html>
<head>
    <title>The Cheesecake Factory</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: beige;
            color: rgb(103, 103, 103);
        }
        
        header {
            background-color: rgb(229, 189, 104);
            color: rgba(0, 0, 0, 0.2);
            text-align: center;
            padding: 1rem;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
        }

        header img {
            border-radius: 50%;
            margin-bottom: 0.5rem;
        }

        header h1 {
            font-size: 2rem;
        }

        header ul {
            list-style: none;
            padding: 0;
        }

        header ul li {
            display: inline;
            margin: 0 10px;
        }

        header a {
            text-decoration: none;
            color: crimson;
            font-weight: bold;
        }

        header a:hover {
            color: white;
        }
        
        main {
            margin: 2rem auto;
            max-width: 900px;
            background: white;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
        }

        .section-heading {
            text-align: center;
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: rgb(66, 64, 64);
            border-bottom: 2px solid crimson;
            padding-bottom: 0.5rem;
        }
        
        article {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1.5rem;
            border-bottom: 1px dashed #ccc;
            padding-bottom: 1rem;
        }

        article img {
            border-radius: 10px;
            width: 120px;
            height: 120px;
            object-fit: cover;
        }

        article h3 {
            font-size: 1.5rem;
            color: #000000;
        }

        .price {
            font-style: italic;
            font-weight: bold;
            color: rgb(152, 150, 150);
        }

        article p {
            margin-top: 0.3rem;
        }

         {
            margin-top: 1.5rem;
            padding: 1rem;
            background-color: #f4f4f4;
            border-radius: 5px;
            box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
        }

        label {
            font-weight: bold;
            display: block;
            margin-top: 0.8rem;
        }

        input[type="number"] {
            width: 100%;
            padding: 0.5rem;
            margin-top: 0.3rem;
            border: 1px solid #a2a2a2;
            border-radius: 5px;
            outline: none;
        }

        input[type="radio"] {
            margin-right: 0.5rem;
        }

        button {
            background-color: crimson;
            color: white;
            padding: 0.8rem 1.5rem;
            border: none;
            border-radius: 5px;
            margin-top: 1rem;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: black;
        }
        
        footer {
            text-align: center;
            margin-top: 1.5rem;
            font-style: italic;
            color: grey;
        }
    </style>
</head>
<body>
<header>
    <img src="https://logodix.com/logo/1073387.png"
         alt="images"
         width="180"
         height="200"
         id="header-img">
    <h1>The Cheesecake Factory</h1>
    <ul>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#order-form">Order Form</a></li>
    </ul>
</header>
<main>
    <section>
        <h2 class="section-heading">Menu</h2>
        <article>
            <img src="https://hips.hearstapps.com/hmg-prod/images/211014-delish-seo-cheesecake-factory-cheesecake-horizontal-050-eb-1635810498.jpg"
                 alt="Cheesecake">
            <div>
                <h3>The Original</h3>
                <p class="price">$3.00</p>
                <p>Our Famous Creamy Cheesecake with a Graham Cracker Crust and Sour Cream Topping</p>
            </div>
        </article>
        <article>
            <img src="https://th.bing.com/th/id/OIP.U8Qh8E6sTXET5xmS_8MtMAHaHa?rs=1&pid=ImgDetMain"
                 alt="Chocolate">
            <div>
                <h3>Chocolate Cake Cheesecake</h3>
                <p class="price">$4.50</p>
                <p>Layer of Our Original Cheesecake, Fudge Cake and Chocolate Truffle Cream</p>
            </div>
        </article>
        <article>
            <img src="https://th.bing.com/th/id/OIP.dBcHVzh9CkCeQFh3510I3QAAAA?rs=1&pid=ImgDetMain"
                 alt="Banana">
            <div>
                <h3>Fresh Banana Cream Cheesecake</h3>
                <p class="price">$3.75</p>
                <p>Banana Cream Cheesecake Topped with Bavarian Cream and Fresh Sliced Bananas</p>
            </div>
        </article>
        <article>
            <img src="https://th.bing.com/th/id/OIP.yCoVCO8ZfCnfj_kAavxYGgHaLI?rs=1&pid=ImgDetMain"
                 alt="Tiramisu">
            <div>
                <h3>Tiramisu Cheesecake</h3>
                <p class="price">$5.75</p>
                <p>Our Wonderful Cheesecake Topped with a Layer of Belgian Chocolate Mousse</p>
            </div>
        </article>
        <article>
            <img src="https://www.cookingclassy.com/wp-content/uploads/2015/11/vanilla_bean_cheesecake13..1.jpg"
                 alt="Vanilla">
            <div>
                <h3>Vanilla Bean Cheesecake</h3>
                <p class="price">$3.50</p>
                <p>Layers of Creamy Vanilla Bean Cheesecake, Vanilla Mousse and Whipped Cream</p>
            </div>
        </article>
    </section>
    <section>
        <h2 class="section-heading">Place Your Order</h2>
        <form id="order-form">
            <label for="cheesecake">The Original:</label>
            <input type="number" id="cheesecake" name="cheesecake" min="0" value="0">

            <label for="chocolate">Chocolate Cake Cheesecake:</label>
            <input type="number" id="chocolate" name="chocolate" min="0" value="0">

            <label for="banana">Fresh Banana Cream Cheesecake:</label>
            <input type="number" id="banana" name="banana" min="0" value="0">

            <label for = "Tiramisu Cheesecake">Tiramisu Cheesecake:</label>
            <input type="number" id="tiramisu" name="Tiramisu Cheesecake" min="0" value="0">

            <label for="Vanilla Bean Cheesecake">Vanilla Bean Cheesecake:</label>
            <input type="number" id="vanilla" name="Vanilla Bean Cheesecake" min="0" value="0">


            <p>Extras for your cheesecake:</p>
            <label>
                <input type="checkbox" name="extras" value="cream" required> Whipped Cream ($0.25)
            </label>
            <label>
                <input type="checkbox" name="extras" value="syrup"> Chocolate syrup ($0.10)
            </label>
            <label>
                <input type="checkbox" name="extras" value="syrup"> Strawberry syrup ($0.10)
            </label>
            <br>
            <textarea cols="30" rows="5" name="Special Requests" placeholder="Special Requests"></textarea>
            <br>
            <br>

            <button type="submit">Go To Checkout</button>
        </form>
    </section>
</main>
<footer>
    <p>Made with love by @ashnair</p>
</footer>
</body>
</html>
