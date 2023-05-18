<style>
    .ripple-border {
        height: 40px;
        background: top center transparent url('/images/ripple-border.svg');
		background-size: cover;
        opacity: .75;
    }
    .ripple-border.bottom {
        transform: scaleY(-1);
    }
    .content-wrapper {
        background: rgba(105,132,146,.75);
    }
    .content-wrapper section {
        max-width: 960px;
        margin: auto;
        min-height: 4em;
        padding: 2em;
    }
</style>
<div>
    <div class="ripple-border top"></div>
    <div class="content-wrapper">
        <section>
            <h1>Value Propisition Goes Here!</h1>
        </section>
    </div>
    <div class="ripple-border bottom"></div>
</div>