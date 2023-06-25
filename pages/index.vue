<template>
    <div class="content-wrap pt-0 pb-0">
        <section class="section mt-0 mb-0">
            <div class="container">
                <div class="row">
                    <div class="col-md-7">
                        <h2 class="display-4 fw-semibold ls--2">
                            We are making better
                            <span
                                class="text-rotater"
                                data-separator="|"
                                data-rotate="fadeIn"
                                data-speed="2000"
                            >
                                <span class="t-rotate"
                                    >Environment|Workspace|CoWorking|Community</span
                                >
                            </span>
                            for you.
                        </h2>
                    </div>
                    <div class="col-md-5">
                        <p class="lead text-muted">
                            Whether you are a freelancer, entrepreneur, or small
                            business owner, we offer the perfect backdrop for
                            creativity, innovation, and collaboration.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <div
            class="overflow-hidden parallax d-flex align-items-center"
            style="height: 600px; width: 100%"
        >
            <img src="demos/coworking/images/hero.jpg" class="parallax-bg" />
            <div class="container">
                <div class="row">
                    <div class="col-lg-6">
                        <h2 class="text-white">
                            Creativity, innovation, and collaboration.
                        </h2>
                    </div>
                </div>
            </div>
        </div>

        <Amenities class="my-0" />

        <CTA
            class="my-0 shadow bg-white border-top border-bottom border-primary"
        />

        <Pricing class="mt-0 pt-6" />

        <section class="section bg-transparent">
            <div class="container">
                <div class="heading-block border-bottom-0 text-center">
                    <div class="before-heading">Gallery</div>
                    <h2 class="text-transform-none fw-semibold mb-0">
                        Life at Noble CoSpace
                    </h2>
                </div>
            </div>
            <div class="container">
                <div
                    class="masonry-thumbs grid-container row row-cols-4"
                    data-big="4"
                    data-lightbox="gallery"
                >
                    <a
                        class="grid-item"
                        :href="image"
                        data-lightbox="gallery-item"
                        v-for="(image, index) in gallery"
                        ><img
                            :src="image"
                            :alt="'Noble CoSpace photo ' + (index + 1)"
                    /></a>
                </div>
            </div>
        </section>
        <section class="section my-0 pb-0">
            <div class="container">
                <div class="row mb-2">
                    <div class="col-lg-6 col-md-4">
                        <div class="heading-block border-bottom-0 mb-4">
                            <div class="before-heading">Location</div>
                            <h2 class="text-transform-none fw-semibold">
                                Visit us
                            </h2>
                        </div>
                    </div>
                </div>
            </div>

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
        <section class="section my-0 py-0">
            <img
                src="@/assets/images/lahore-silhouette.png"
                alt="Footer Image"
                class="w-100"
                style="opacity: 0.8"
            />
        </section>
        <MiniCTA>
            Need 1 Day Trial for Free? <strong>Reserve Now</strong>
        </MiniCTA>
    </div>
</template>

<script>
import { formatNumber } from "humanize-plus";
export default {
    name: "Index",
    head: {
        title: "noble cospace",
    },
    data() {
        return {
            rates: [
                {
                    title: "Flexible Desk",
                    tagline: "Economical but flexible.",
                    price: 12000,
                    price_duration: "month",
                    features: ["8hr/day", "Free Tea/Coffee"],
                },
                {
                    title: "Dedicated Desk",
                    tagline: "Your personal desk.",
                    price: 15000,
                    price_duration: "month",
                    features: [
                        "12hr/day",
                        "Free Tea/Coffee",
                        "Meeting Room Credits",
                        "Personal Locker",
                        "Mail Handling",
                    ],
                },
                {
                    title: "Private Office",
                    tagline: "It's all yours.",
                    price: 18000,
                    price_duration: "month",
                    features: [
                        "12hr/day",
                        "Free Tea/Coffee",
                        "Meeting Room Credits",
                        "Personal Lockers",
                        "Mail Handling",
                        "Office Customization",
                        "Printing Credits",
                    ],
                },
            ],
            gallery: [
                "demos/coworking/images/gallery/1.jpg",
                "demos/coworking/images/gallery/2.jpg",
                "demos/coworking/images/gallery/3.jpg",
                "demos/coworking/images/gallery/4.jpg",
                "demos/coworking/images/gallery/5.jpg",
                "demos/coworking/images/gallery/6.jpg",
                "demos/coworking/images/gallery/7.jpg",
                "demos/coworking/images/gallery/8.jpg",
                "demos/coworking/images/gallery/9.jpg",
                "demos/coworking/images/gallery/10.jpg",
                "demos/coworking/images/gallery/11.jpg",
                "demos/coworking/images/gallery/12.jpg",
                "demos/coworking/images/gallery/13.jpg",
                "demos/coworking/images/gallery/14.jpg",
                "demos/coworking/images/gallery/15.jpg",
            ],
        };
    },
    methods: {
        formatNumber,
    },
};
</script>
<style lang="scss">
.map-container {
    height: 600px;
}
// #section-purchase {
//     .background-container {
//         padding: 150px 0;
//         background: url("@/assets/images/lahore-silhouette.png") no-repeat
//             center 320px;
//         background-size: contain;
//         height: 760px;
//     }
//     .container {
//         background: rgba(255, 255, 255, 0.8);
//     }
// }
</style>
