  <head>
    <meta charset="UTF-8" />
    <link rel="icon" type="image/svg+xml" href="vite.svg" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Daily Tarot Reading</title>

    <!-- Tailwind -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Source+Sans+3:wght@300;400&display=swap" rel="stylesheet">

    <style>
      body {
        font-family: 'Source Sans 3', sans-serif;
        background-color: #fdf2f8;
        background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='40' height='40' viewBox='0 0 40 40'%3E%3Cg fill-rule='evenodd'%3E%3Cg fill='%23fbcfe8' fill-opacity='0.2'%3E%3Cpath d='M0 38.59l2.83-2.83 1.41 1.41L1.41 40H0v-1.41zM0 1.4l2.83 2.83 1.41-1.41L1.41 0H0v1.41zM38.59 40l-2.83-2.83 1.41-1.41L40 38.59V40h-1.41zM40 1.41l-2.83 2.83-1.41-1.41L38.59 0H40v1.41zM20 18.6l2.83-2.83 1.41 1.41L21.41 20l2.83 2.83-1.41 1.41L20 21.41l-2.83 2.83-1.41-1.41L18.59 20l-2.83-2.83 1.41-1.41L20 18.59z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
      }
      h1, h2, h3 {
        font-family: 'Playfair Display', serif;
      }
      @keyframes titleFadeIn {
        from { opacity: 0; transform: translateY(-10px); }
        to { opacity: 1; transform: translateY(0); }
      }
      .animate-title-fade-in {
        animation: titleFadeIn 0.8s ease-out forwards;
        opacity: 0;
      }
    </style>

    <!-- Import maps for React + Google GenAI -->
    <script type="importmap">
    {
      "imports": {
        "@google/genai": "https://aistudiocdn.com/@google/genai@^1.29.1",
        "react-dom/": "https://aistudiocdn.com/react-dom@^19.2.0/",
        "react/": "https://aistudiocdn.com/react@^19.2.0/",
        "react": "https://aistudiocdn.com/react@^19.2.0"
      }
    }
    </script>
  </head>

  <body>
    <div id="root"></div>

    <!-- IMPORTANT: In GitHub Pages, do not use leading slash -->
    <script type="module" src="index.tsx"></script>
  </body>
</html>
