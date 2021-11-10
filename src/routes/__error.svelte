<style lang="scss">
    .error {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100vh;
        width: 100vw;
        background-image: url('buster_keaton.gif');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
    }

    .text {
        color: #fff;
        text-shadow: 1px 1px #283229;
        font-family: 'Cutive Mono';
        position: relative;
        text-align: center;
        max-width: calc(100% - 1rem);
        
        @media screen and (min-width: 768px) {
            font-size: 1.5rem;
            line-height: 2rem;
        }
    
        @media screen and (min-width: 1280px) {
            font-size: 1.75rem;
            line-height: 2.1875rem;
        }
    }
</style>

<div class="error">
    <h1 class="text">404: Page Not Found</h1>
</div>