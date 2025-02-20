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
