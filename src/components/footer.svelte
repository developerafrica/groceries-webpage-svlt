<article class="footer">
    <div class="art-ft">
        <header>
            <h1>created with 🖤 by <a href="https//github.com/peterbutao">PETER BUTAO | DEVELOPER AFRICA MW</a></h1>
        </header>
        <main>
            <div class="mn">

            </div>
        </main>
        <footer>
            <p>&copy peterbutao|developerafricamw2023</p>
        </footer>
    </div>
</article>
<style lang="scss">
    article{
        text-align: center;
        .art-ft{
            header{
                h1{
                    @include fnt(var(--tc), 0.7rem, 500);
                    a{
                        @include fnt(var(--gn), 0.7rem, 500);
                        text-decoration: none;
                    }
                }
            }
            footer{
                p{
                    @include fnt(var(--tc), 0.7rem, 500);

                }
            }
        }
    }
</style>