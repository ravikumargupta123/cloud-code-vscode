# PWA and webaccessibility

- install service worker paste below code in index.html
    ```
        <script>
            if ('serviceWorker' in navigator) {
                window.addEventListener('load', function() {
                    navigator.serviceWorker.register('sw.js')
                    .then(reg => {
                        console.log('Service worker registered! 😎', reg);
                    })
                    .catch(err => {
                        console.log('😥 Service worker registration failed: ', err);
                    });
                });
            }
	    </script>

    ```
