<template>
    <div>
        <div class="container my-6">
            <div class="row justify-content-center text-center">
                <div class="col-md-12">
                    <h1 class="display-4 text-dark fw-semibold ls--2">
                        Flexible Membership Options
                    </h1>
                    <p class="text-dark">
                        Find the Perfect Plan for Your Workspace Needs
                    </p>
                    <NuxtLink
                        to="/forms/membership"
                        class="button button-rounded button-large m-0 text-center fw-medium text-transform-none ls-0 fw-normal"
                        >Book your Free Trial</NuxtLink
                    >
                </div>
            </div>
        </div>
        <Pricing class="mb-0" />
        <CTA
            class="my-0 shadow bg-white border-top border-bottom border-primary"
        />

        <Amenities class="bg-white mb-0 pb-0" />
        <section class="section mb-0">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div class="text-center">
                            <div class="before-heading">FAQ</div>
                        </div>
                        <h2 class="text-dark text-center fw-semibold ls--2">
                            Frequently Asked Questions
                        </h2>
                        <p class="text-center">
                            Here are some of the most common questions we get
                            asked.
                        </p>
                        <div
                            class="accordion accordion-flush"
                            id="faqAccordion"
                            data-collapsible="true"
                        >
                            <template v-for="(item, i) in faq">
                                <div class="accordion-header">
                                    <div
                                        class="accordion-title"
                                        v-text="item.question"
                                    ></div>
                                </div>
                                <div
                                    class="ms-2 accordion-content"
                                    v-html="item.answer"
                                ></div>
                            </template>
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
    data() {
        return {
            faq: [
                {
                    question:
                        "What are the payment terms for the membership plans?",
                    answer: "We offer flexible payment options for our membership plans. You can choose to pay on a monthly, semi-annually, or annually, depending on your preference and convenience. Our team will provide you with all the necessary details and assist you in selecting the best payment plan for your needs.",
                },
                {
                    question: "Can I upgrade or downgrade my membership plan?",
                    answer: "Yes, you can upgrade or downgrade your membership plan at any time. We understand that your workspace needs may change over time, and we are here to accommodate those changes. Simply get in touch with our team, and we will guide you through the process.",
                },
                {
                    question:
                        "Are there any additional fees apart from the membership costs?",
                    answer: "Our membership plans are designed to be transparent and all-inclusive. However, there may be additional charges for certain services or amenities that are not covered under the standard membership. These charges will be clearly communicated to you in advance, ensuring there are no surprises.",
                },
                {
                    question:
                        "Can I use the coworking space during weekends and after office hours?",
                    answer: "Yes, our coworking space is accessible 24/7, including weekends and after office hours. We understand that our members have different working styles and schedules, so we provide round-the-clock access to ensure maximum flexibility and convenience.",
                },
                {
                    question:
                        "What amenities are included in the membership plans?",
                    answer: "Refer to the plan details above for a complete list of amenities included in each membership plan. If you have any specific requirements, please get in touch with our team, and we will be happy to assist you.",
                },
                {
                    question:
                        "Can I bring guests or clients to the coworking space?",
                    answer: "Absolutely! We encourage our members to invite guests or clients to our coworking space. Whether it's for a meeting, collaboration, or simply to showcase your office, we welcome your guests and provide a professional environment for all.",
                },
            ],
        };
    },
};
</script>
