<article class="contact">
    <div class="art-cnt">
        <header>
            <h1>have something in mind ?</h1>
        </header>
        <main>
            <div class="contact">
                <a href="tel://0880164455">CONTACT</a>
            </div>
        </main>
        <footer>
            <div class="ft">
                <div class="image">
                    <img src="/businesscard.png" alt="business card">
                </div>
                <div class="download">
                    <a href="/businesscard.png" download="business card">DOWNLOAD OUR BUSINESS CARD &rarr;</a>
                </div>
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
        padding: 20px 0;
        .art-cnt{
            text-align: center;
            padding: 20px;
            header{
                h1{
                    @include fnt(var(--tc), 0.8rem, 500);
                    letter-spacing: 1.3px;
                   
                    
                }
            }
            main{
                .contact{
                    padding: 10px 20px;
                    a{
                        display: block;
                        @include fnt(var(--tc), 1rem, 500);
                        border: var(--gn) solid 1px;
                        padding: 10px;
                        text-decoration: none;
                    }
                }
            }
            footer{
                .ft{
                    .image{
                        padding: 20px 0;
                        width: 300px;
                        margin: auto;
                        img{
                            width: 100%;
                            box-shadow: rgba(0, 0, 0, 0.182) 0 4px 4px 0;
                        }
                    }
                    .download{
                        padding: 20px 0;
                        a{
                            text-decoration: none;
                            @include fnt(var(--gn), 0.75rem, 450);
                           

                        }
                    }
                }
            }
        }
    }
</style>