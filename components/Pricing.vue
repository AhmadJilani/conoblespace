<template>
    <section class="section">
        <div class="container">
            <header class="section-header">
                <div class="heading-block mb-4 border-bottom-0">
                    <div class="before-heading">Rates</div>
                    <h2 class="text-transform-none fw-semibold">
                        Flexible workspace solutions
                    </h2>
                </div>
            </header>

            <div class="row">
                <div class="col-12">
                    <div class="promo promo-light p-4 p-md-5 mb-5">
                        <div class="row align-items-center">
                            <div class="col-12 col-lg">
                                <h3>
                                    20% off introductory discount for the first
                                    6 months
                                </h3>
                                <p>
                                    This discount is valid for a limited time
                                    only; applicable on all membership plans.
                                </p>
                            </div>
                            <div class="col-12 col-lg-auto mt-4 mt-lg-0">
                                <NuxtLink
                                    to="/forms/membership"
                                    class="button button-large button-circle button-black m-0"
                                >
                                    Reserve Now
                                </NuxtLink>
                            </div>
                        </div>
                    </div>
                    <div
                        id="price-carousel"
                        class="owl-carousel carousel-widget"
                        data-margin="30"
                        data-nav="false"
                        data-pagi="true"
                        data-items-xs="1"
                        data-items-sm="1"
                        data-items-md="2"
                        data-items-lg="3"
                        data-items-xl="3"
                    >
                        <div
                            class="price-list shadow-sm card border-0 rounded"
                            v-for="rate in rates"
                        >
                            <div class="position-relative">
                                <img
                                    :src="
                                        rate.image ||
                                        'demos/coworking/images/membership/share.jpg'
                                    "
                                    :alt="rate.title"
                                    class="card-img-top rounded-top"
                                />
                                <div
                                    class="card-img-overlay dark d-flex justify-content-center flex-column p-0 text-center"
                                >
                                    <h3
                                        class="card-title mb-0 text-white"
                                        v-text="rate.title"
                                    ></h3>
                                    <p
                                        class="card-text mb-0"
                                        v-text="rate.tagline"
                                    ></p>
                                </div>
                            </div>
                            <div class="card-body">
                                <div
                                    class="text-muted h3 mb-0"
                                    v-if="rate.discounted_price"
                                >
                                    <del
                                        >Rs.
                                        {{ formatNumber(rate.price) }}
                                    </del>
                                    <span
                                        class="badge bg-secondary shadow-sm ms-2"
                                        v-if="rate.discounted_price"
                                    >
                                        20% off
                                    </span>
                                </div>
                                <div class="price-title pb-3">
                                    Rs.
                                    {{
                                        formatNumber(
                                            rate.discounted_price || rate.price
                                        )
                                    }}
                                    <small>PKR/{{ rate.price_duration }}</small>
                                </div>

                                <ul
                                    class="list-group list-group-flush mb-4"
                                    v-if="rate.features && rate.features.length"
                                >
                                    <li
                                        class="list-group-item ps-0"
                                        v-for="feature in rate.features"
                                    >
                                        <i class="bi-check-lg pe-3 color"></i>
                                        {{ feature }}
                                    </li>
                                </ul>

                                <NuxtLink
                                    to="/forms/membership"
                                    class="button button-rounded button-large w-100 m-0 text-center fw-medium"
                                    >Join Now</NuxtLink
                                >
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import { formatNumber } from "humanize-plus";
export default {
    name: "Pricing",
    data() {
        return {
            rates: [
                {
                    title: "Flexible Desk",
                    tagline: "Economical but flexible.",
                    price: 18000,
                    discounted_price: 18000 * 0.8,
                    price_duration: "month/seat",
                    features: ["12hr/day", "Free Tea/Coffee"],
                },
                {
                    title: "Dedicated Desk",
                    tagline: "Your personal desk.",
                    price: 22000,
                    discounted_price: 22000 * 0.8,
                    price_duration: "month/seat",
                    features: [
                        "24hr/day",
                        "Free Tea/Coffee",
                        "Meeting Room Credits",
                        "Personal Locker",
                        "Mail Handling",
                    ],
                },
                {
                    title: "Private Office",
                    tagline: "It's all yours.",
                    price: 26000,
                    discounted_price: 26000 * 0.8,
                    price_duration: "month/seat",
                    features: [
                        "24hr/day",
                        "Free Tea/Coffee",
                        "Meeting Room Credits",
                        "Personal Lockers",
                        "Mail Handling",
                        "Office Customization",
                        "Printing Credits",
                    ],
                },
                {
                    title: "Day Pass",
                    tagline: "For a day.",
                    price: 1500,
                    price_duration: "day/seat",
                    features: ["8hr/day", "Basic Amenities"],
                },
                {
                    title: "Meeting Room",
                    tagline: "For your meetings.",
                    price: 2000,
                    price_duration: "hour",
                    features: ["Free Tea/Coffee", "Fully Equipped Room"],
                },
                {
                    title: "Virtual Office",
                    tagline: "Your business address.",
                    price: 6000,
                    price_duration: "month",
                    features: ["Business Address", "Mail Handling"],
                },
            ],
        };
    },
    methods: {
        formatNumber,
    },
};
</script>
