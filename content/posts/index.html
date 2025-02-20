<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Blog</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 40px; text-align: center; }
        .post { border-bottom: 1px solid #ccc; padding: 20px; }
    </style>
</head>
<body>
    <h1>Bem-vindo ao Meu Blog</h1>
    <div id="posts"></div>
    
    <script>
        async function loadPosts() {
            const response = await fetch('posts.json'); // JSON com links dos arquivos .md
            const posts = await response.json();
            const postsContainer = document.getElementById('posts');
            
            posts.forEach(async post => {
                const postResponse = await fetch(post.url);
                const postText = await postResponse.text();
                
                const postElement = document.createElement('div');
                postElement.className = 'post';
                postElement.innerHTML = `<h2>${post.title}</h2><p>${postText.substring(0, 200)}...</p>`;
                postsContainer.appendChild(postElement);
            });
        }
        
        loadPosts();
    </script>
</body>
</html>
