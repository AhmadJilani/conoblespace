<template>
    <div>
        <div class="container my-6">
            <div class="row justify-content-center text-center">
                <div class="col-md-8">
                    <h1 class="display-4 text-dark fw-semibold ls--2">
                        Contact Us
                    </h1>
                    <p>Reach out to us and we'll respond as soon as we can.</p>
                </div>
            </div>
        </div>

        <section class="section mb-0">
            <div class="container">
                <div class="row align-items-stretch col-mb-50 mb-0">
                    <div class="col-lg-6">
                        <div class="fancy-title title-border">
                            <h3>Send us an Email</h3>
                        </div>
                        <div>
                            <iframe
                                data-tally-src="https://forms.noblecospace.com/contact?hideTitle=1&transparentBackground=1&dynamicHeight=1&embed=1"
                                loading="lazy"
                                width="100%"
                                height="324"
                                frameborder="0"
                                marginheight="0"
                                marginwidth="0"
                                title="Contact"
                            ></iframe>
                        </div>
                    </div>

                    <div class="col-lg-6 min-vh-50">
                        <div class="position-relative map-container">
                            <iframe
                                src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d13604.137429122837!2d74.317006!3d31.5232163!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x391905d79978b6fd%3A0x67ff390983c234db!2snoble%20cospace!5e0!3m2!1sen!2s!4v1687718596380!5m2!1sen!2s"
                                allowfullscreen
                                style="border: 0"
                                class="w-100 h-100"
                            ></iframe>
                        </div>
                    </div>
                </div>

                <div class="row col-mb-50 mb-4">
                    <div class="col-sm-6 col-lg-6">
                        <div
                            class="feature-box fbox-center fbox-bg fbox-plain border-secondary"
                        >
                            <div class="fbox-icon bg-light">
                                <NuxtLink to="/location"
                                    ><i class="uil uil-map-marker"></i
                                ></NuxtLink>
                            </div>
                            <div class="fbox-content">
                                <h3>
                                    Visit Us<span class="subtitle"
                                        >337, Rehmanpura, Lahore</span
                                    >
                                </h3>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-6 col-lg-6">
                        <div
                            class="feature-box fbox-center fbox-bg fbox-plain border-secondary"
                        >
                            <div class="fbox-icon bg-light">
                                <a href="tel:+924232803320"
                                    ><i class="bi-telephone"></i
                                ></a>
                            </div>
                            <div class="fbox-content">
                                <h3>
                                    Speak to Us<span class="subtitle"
                                        >+92 423 2803320</span
                                    >
                                </h3>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <MiniCTA>
            Need 1 Day Trial for Free? <strong>Reserve Now</strong>
        </MiniCTA>
    </div>
</template>
<script>
export default {
    head() {
        return {
            title: "Contact | noble cospace",
            meta: [
                {
                    hid: "description",
                    name: "description",
                    content:
                        "Contact us for any queries regarding our work space.",
                },
            ],
        };
    },
    data() {
        return {};
    },
    methods: {},
    mounted() {
        var d = document,
            w = "https://tally.so/widgets/embed.js",
            v = function () {
                "undefined" != typeof Tally
                    ? Tally.loadEmbeds()
                    : d
                          .querySelectorAll("iframe[data-tally-src]:not([src])")
                          .forEach(function (e) {
                              e.src = e.dataset.tallySrc;
                          });
            };
        if ("undefined" != typeof Tally) v();
        else if (d.querySelector('script[src="' + w + '"]') == null) {
            var s = d.createElement("script");
            (s.src = w), (s.onload = v), (s.onerror = v), d.body.appendChild(s);
        }
    },
};
</script>
