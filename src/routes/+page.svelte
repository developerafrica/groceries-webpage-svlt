<article class="main">
    <div class="art-main">
        <main>
            <img src="/phonedesign.png" alt="phone design">
        </main>
        <footer>
            <div class="text">
                <p>do you still write your groceries on paper ?</p>
                <h1>this app is for you</h1>
            </div>
        </footer>
    </div>
</article>
<style lang="scss">
    @mixin fnt ($c,$s,$w) {
    font-size: $s;
    color: $c;
    font-weight: $w;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    
    
}
    article{
        .art-main{
            padding: 10vh 0 0 0;
            main{
                margin: auto;
                width: 300px;
                img{
                    margin: auto;
                    width: 100%;
                    padding: 10px;
                }
            }
            footer{
                padding: 10px;
                text-align: center;
                .text{
                    p{
                        @include fnt(var(--tc), 0.78rem, 500);
                    }
                    h1{
                        @include fnt(var(--tc), 0.9rem, 800);
                        text-transform: uppercase;
                        letter-spacing: 1.5px;
                    }
                }

            }

        }
    }
</style>