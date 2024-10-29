<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Explore the Stars ✨</title>
    <style>
        /* Basic page settings */
        body, html {
            margin: 0;
            padding: 0;
            overflow: hidden;
            font-family: Arial, sans-serif;
            color: white;
            perspective: 1px;
            height: 100vh;
            overflow-x: hidden;
            background-color: #000;
        }

        /* 3D Layered Starry Sky Background */
        .parallax {
            position: relative;
            height: 100vh;
            transform-style: preserve-3d;
        }

        .layer {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-size: cover;
            background-position: center;
            animation: moveLayers 30s infinite linear;
        }

        .layer1 {
            background-image: url('https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwzNjUyOXwwfDF8c2VhcmNofDV8fHN0YXJyeSUyMG5pZ2h0fGVufDB8fHx8MTY3ODczNzg5OA&ixlib=rb-1.2.1&q=80&w=1080');
            transform: translateZ(-2px) scale(3);
            opacity: 0.4;
        }

        .layer2 {
            background-image: url('https://images.unsplash.com/photo-1551672742-a9b2a4a9eacf');
            transform: translateZ(-1px) scale(2);
            opacity: 0.6;
        }

        .layer3 {
            background-image: url('https://images.unsplash.com/photo-1519038396812-0d3f10f7f6e2');
            transform: translateZ(0px) scale(1);
            opacity: 0.8;
        }

        /* Text content styling */
        .content {
            position: relative;
            z-index: 100;
            text-align: center;
            padding: 40px;
        }

        h1 {
            font-size: 4em;
            color: #ffcccb;
            margin: 0;
            text-shadow: 0px 0px 20px #ffcccb;
        }

        p {
            font-size: 1.2em;
            color: #f1f1f1;
            max-width: 600px;
            margin: 20px auto;
        }

        /* Animations for layers */
        @keyframes moveLayers {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }

    </style>
</head>
<body>

    <!-- Parallax background layers -->
    <div class="parallax">
        <div class="layer layer1"></div>
        <div class="layer layer2"></div>
        <div class="layer layer3"></div>
    </div>

    <!-- Content Section -->
    <div class="content">
        <h1>The Stars & Beyond 🌌</h1>
        <p>
            Journey through the cosmic clouds, where stars are born and shine their light across the universe. Discover the magic of nebulae, 
            galaxies, and everything in between. Each layer of stars brings you closer to understanding the vastness and wonder of space.
        </p>
    </div>
</body>
</html>
