<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    main {
        gap: 20px;
        padding: 20px;
    }

    body {
        background-color: black;
    }

    header {
        background-color: white;
        height: 50px;
        font-size: 30px;
    }

    article {
        background-color: antiquewhite;
        height: 500px;
        font-size: 20px;
    }

    aside {
        background-color: aquamarine;
        height: 500px;
        font-size: 20px;
    }

    footer {
        background-color: antiquewhite;
        height: 50px;
        font-size: 20px;
    }

    main {
        display: grid;
        grid-template-areas:
            "head head head head head"
            "side content content content content"
            "foot foot foot foot foot";
    }

    header {
        grid-area: head;
    }

    article {
        grid-area: content;
    }

    aside {
        grid-area: side;
    }

    footer {
        grid-area: foot;
    }

    @media screen and (max-width:500px) {
        header {
            font-size: 20px;
        }

        aside {
            display: none;
        }

        main {

            grid-template-areas:
                "head head "
                "content content "
                "foot foot ";
        }
    }
</style>

<body>
    <main>
        <header>HEY!!... This is My First Website</header>
        <article>
            Content
        </article>
        <aside>Sidebar</aside>
        <footer>Footer</footer>
    </main>
</body>

</html>
