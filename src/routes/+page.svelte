<script>
    import Contact from "../components/contact.svelte"
    import Footer from "../components/footer.svelte"
</script>
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
        <hr>
        <section class="launch">
            <div class="card">
                <header>
                    <div class="image">
                        <svg width="100" height="100" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <rect width="100" height="100" rx="5" fill="white"/>
                            <path d="M35 35C35 29.4737 30.5263 25 25 25C23.6404 25 22.5 26.1404 22.5 27.5C22.5 28.8596 23.6404 30 25 30C28.0702 30 30 31.9298 30 35C30 36.3596 31.1404 37.5 32.5 37.5C33.8596 37.5 35 36.3596 35 35ZM63.5088 37.5C67.0175 37.5 69.0351 39.9561 68.4211 43.4211L66.1842 55.921C65.7018 58.5526 63.9474 60 61.2281 60H40C36.9298 60 35 58.0702 35 55V37.5H63.5088ZM63.5088 32.5H30V55C30 60.5263 34.4737 65 40 65H61.2281C66.0526 65 70.2193 61.5351 71.0965 56.7982L73.3333 44.2982C74.4298 38.1579 69.7807 32.5 63.5088 32.5ZM62.5 67.5C59.7368 67.5 57.5 69.7368 57.5 72.5C57.5 75.2632 59.7368 77.5 62.5 77.5C65.2632 77.5 67.5 75.2632 67.5 72.5C67.5 69.7368 65.2632 67.5 62.5 67.5ZM37.5 67.5C34.7368 67.5 32.5 69.7368 32.5 72.5C32.5 75.2632 34.7368 77.5 37.5 77.5C40.2632 77.5 42.5 75.2632 42.5 72.5C42.5 69.7368 40.2632 67.5 37.5 67.5Z" fill="#113C11"/>
                        </svg>
                            
                    </div>
                    <div class="text">
                        <h1>BUDGET APP</h1>
                        <p>SIMPLIFY BUDGETING AND CALCULATIONS FOR GROCERIES </p>
                    </div>
                </header>
                <main>
                    <div class="ft"><a href="https://budgetonline.netlify.app/">LAUNCH ONLINE &rarr;</a></div>
                </main>
            </div>
        </section>
        <section class="footer-section">
            <Contact />
            <Footer />
        </section>
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
        max-width: 800px;
        margin: auto;
        .art-main{
            padding: 10vh 0 0 0;
            main{
                margin: auto;
                width: 250px;
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
            .launch{
                background: gold;
                padding: 10px;
                margin: 15vh 10px;
                border-radius: 4px;
                header{
                    display: flex;
                    align-items: center;
                    justify-content: space-between;
                    gap: 10px;
                    .image{
                        svg{
                            width: 60px;
                        }
                    }
                    .text{
                        h1{
                            @include fnt(var(--tc), 1rem, 700);
                            margin: 0;
                            letter-spacing: 1.3px;
                            padding: 0;
                        }
                        p{
                            @include fnt(var(--tc), 0.7rem, 600)
                        }
                    }
                }
                main{
                    width: 100%;
                    .ft{
                        a{
                            display: block;
                            text-decoration: none;
                            background: var(--tc);
                            text-align: center;
                            @include fnt(var(--wt), 1rem, 500);
                            padding: 15px;
                            border-radius: 5px;
                        }
                    }
                }

            }
            .footer-section{
                background: rgba(0, 0, 0, 0.1);
                padding: 10px 0 30vh 0;
            }

        }
    }
</style>