<script lang="ts">

</script>
<style>
    footer.footer section {
        background: rgba(105,132,146,1);
    }
    div.ripple-border {
        height: 40px;
        background: top center transparent url('/images/ripple-border.svg');
		background-size: cover;
       
    }
    div.ripple-line {
        background: top center transparent url('/images/ripple-line.svg') no-repeat;
        background-size: 100%;
        height: 40px;
    }
    div.ripple-line-blue {
        background: top center transparent url('/images/ripple-line-blue.svg') no-repeat;
        background-size: 100%;
        height: 40px;
    }
    footer.footer .bottom {
        display: flex;
        align-items: center;
        padding-left: 2em;
    }
    footer.footer .bottom img {
        width: 2em;
        height: 2em;
    }
    div.footer-link {
        text-align: right;
        line-height: 2;
        padding: 2em;
        font-size: 0.9em;
        margin-left: auto;
    }
    div.footer-link a {
        color: white;
        text-decoration: none;
    }
    div.footer-link a:hover {
        text-decoration: underline;
    }
    .footer-cta {
        display: flex;
        padding: 2em;
        max-width: 960px;
        margin: auto;
        align-items: center;
    }
    .footer-cta .copy {
        font-size: 2em;
        font-weight: bold;
        color: #EBE8CC;
    }
    .donate {
        max-width: 960px;
        margin: auto;
        padding: 4em 0;
    }
    .donate .copy {
        font-size: 2em;
        font-weight: bold;
        color: #3E5F72;
    }
    .footer-cta button {
        background: #EBE8CB;
        border-radius: 5px;
        color: rgba(105,132,146,1);
        font-size: 1em;
        border: none;
        font-weight: bold;
        padding: 1em 3em;
    }
    .footer-cta .button-wrap {
        margin-left: auto;
    }
    @media (max-width: 950px) {
        .donate {
            padding: 4rem 2rem;
        }
    }
</style>
<footer class="footer">
    <div class="ripple-line-blue"></div>
    <div class="donate">
        <div class="copy">
            <span>Cras fringilla dolor vitae justo,<br> aliquet ultricies tortor aliquam.</span>
        </div>
    </div>
    <div class="ripple-border top"></div>
    <section>
        <div class="footer-cta">
            <div class="copy">
                <span>Join our Discord lorem<br> ipsum dolor sit amet</span>
            </div>
            <div class="button-wrap">
                <button>Join Now</button>
            </div>
        </div>
        <div class="ripple-line"></div>
        <div class="bottom">
            <img src="/images/logo-small.png" alt="Impact Stream" />
            <div class="footer-link"><a href="mailto:hello@impact.stream">hello@impact.stream</a></div>
        </div>
    </section>
</footer>