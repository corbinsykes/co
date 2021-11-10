<style lang="scss">
    :root {
        --white: #FFF;
        --green: #33E866;
        --shadow: #283229;

        --text-shadow: 1px 1px;
        --box-shadow: 0 2px 4px;
    }
    
    .page,
    .content,
    .links,
    .link {
        display: flex;
        align-items: center;
    }

    .page,
    .content {
        justify-content: center;
    }

    .content,
    .links {
        flex-direction: column;
    }

    .page {
        height: 100vh;
        width: 100vw;
    }

    .content {
        position: relative;
        height: 100%;
        width: 100%;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        transition: filter 0.375s cubic-bezier(0.6, 0.04, 0.98, 0.335);
        
        @media screen and (min-width: 768px) {
            border-radius: 0.5rem;
            box-shadow: 0 2px 4px #283229;
        }
    }

    .video {
        filter: brightness(0.667);
        position: fixed;
        top: 0;
        right: 0;
        bottom: 0;
        left: -125%;
        min-height: 100%;
        min-width: 100%;

        @media screen and (min-width: 768px) {
            left: -67%;
        }

        @media screen and (min-width: 1024px) {
            left: -25%;
        }

        @media screen and (min-width: 1800px) {
            left: 0;
        }
    }

    .text,
    [class^="fa"] {
        color: #fff;
        font-size: 1rem;
        line-height: 1.5rem;
        text-shadow: 1px 1px #283229;
        transition: text-shadow 0.5s ease;
    }
    
    .text {
        font-family: 'Cutive Mono';
        position: relative;
        text-align: center;
        max-width: calc(100% - 1rem);
        
        &--title {
            @media screen and (min-width: 768px) {
                font-size: 1.5rem;
                line-height: 2rem;
            }
        
            @media screen and (min-width: 1280px) {
                font-size: 1.75rem;
                line-height: 2.1875rem;
            }
        }
    }

    .links {
        gap: 1.5rem;
        margin-top: 1.5rem;

        @media screen and (min-width: 768px) {
            flex-direction: row;
            gap: 2.5rem;
            margin-top: 4rem;
        }
    }

    .link {
        gap: 0.75rem;
        cursor: pointer;
        position: relative;


        &:hover {
            .text,
            [class^="fa"] {
                color: #fff;
                text-shadow: 1px 1px #33E866;
            }
        }
    }
</style>

<section class="page">
    <div class="content">
        <video
            class="video"
            autoplay
            muted
            loop
            poster="zaouli.gif">
            <source src="zaouli.mp4" type="video/mp4">
        </video>

        <h1 class="text text--title">Corbin Elliott:</h1>
        <h1 class="text text--title">writes javascript, CSS,</h1>
        <h1 class="text text--title">and random haikus.</h1>

        <div class="links">
            <a class="link" href="https://github.com/corbinsykes">
                <i class="fab fa-github-alt"></i>
                <p class="text text--link">github</p>
            </a>

            <a class="link" href="https://linkedin.com/in/corbinsykes">
                <i class="fab fa-linkedin-in"></i>
                <p class="text text--link">linkedin</p>
            </a>

            <a class="link" href="mailto:corbin.sykes@gmail.com">
                <i class="far fa-envelope"></i>
                <p class="text text--link">email</p>
            </a>

            <a class="link" href="tel:2163861880">
                <i class="fas fa-mobile-alt"></i>
                <p class="text text--link">phone</p>
            </a>

            <a class="link" href="Resume.pdf" download="Corbin Sykes - Resume">
                <i class="fas fa-file-download"></i>
                <p class="text text--link">resume</p>
            </a>
        </div>
    </div>
</section>
