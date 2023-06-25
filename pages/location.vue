<template>
    <div>
        <div class="container my-6">
            <div class="row justify-content-center text-center">
                <div class="col-md-8">
                    <h1 class="display-4 text-dark fw-semibold ls--2">
                        Find Us in the Heart of the City
                    </h1>
                    <p>
                        Whether you're commuting from downtown, nearby
                        neighborhoods, or even from the outskirts, our central
                        location ensures a hassle-free commute for you and your
                        team.
                    </p>
                </div>
            </div>
        </div>

        <MiniCTA>
            Need 1 Day Trial for Free? <strong>Contact Now</strong>
        </MiniCTA>
        <section class="section my-0 pb-0">
            <div class="position-relative map-container">
                <iframe
                    src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d13604.137429122837!2d74.317006!3d31.5232163!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x391905d79978b6fd%3A0x67ff390983c234db!2snoble%20cospace!5e0!3m2!1sen!2s!4v1687718596380!5m2!1sen!2s"
                    allowfullscreen
                    style="border: 0"
                    class="w-100 h-100"
                ></iframe>
            </div>

            <div class="hero-features col-md-6 shadow shadow-sm bg-white">
                <div class="row lead">
                    <div class="col-md-6">
                        <h3 class="mb-4">
                            <i class="bi-geo-alt pe-2"></i>
                            Address
                        </h3>
                        <address>
                            337 G, Rehman Pura<br />Lahore 54000,<br />Pakistan
                        </address>
                    </div>
                    <div class="col-md-6">
                        <h3 class="mb-4">
                            <i class="bi-telephone pe-2"></i>
                            Contact
                        </h3>
                        <small class="text-black-50">Phone Number</small>
                        <br />
                        <a href="tel:+923238878361">0323 8878361</a>
                        <br />
                        <small class="text-black-50">Email</small>
                        <br />
                        <a href="mailto:info@noblecospace.com">
                            info@noblecospace.com
                        </a>
                    </div>
                    <div class="col-md-3"></div>
                </div>
            </div>
        </section>
        <CTA
            class="my-0 shadow bg-white border-top border-bottom border-primary"
        />
    </div>
</template>
<script>
export default {
    data() {
        return {};
    },
};
</script>
