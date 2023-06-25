<template>
    <div class="section">
        <div class="container">
            <div class="row justify-content-between align-items-center">
                <!-- <div class="col-lg-8 col-md-10 offset-lg-2 offset-md-1 mb-6">
                    <a
                        href="https://www.youtube.com/watch?v=bZK_0FxL2iM"
                        data-lightbox="iframe"
                        class="play-video position-relative"
                        ><img
                            src="demos/coworking/images/video-bg.jpg"
                            alt="Video Image"
                            class="rounded-3 shadow-lg"
                        />
                        <i class="bi-play"></i>
                    </a>
                </div> -->
                <div class="col-lg-5 col-md-6 mt-0 mt-md-4">
                    <div class="feature-box fbox-plain fbox-sm">
                        <div class="fbox-icon">
                            <i class="bi-magic"></i>
                        </div>
                        <div class="fbox-content">
                            <h3>Discover Your Perfect Workspace</h3>
                            <p>
                                Whether you're a freelancer, entrepreneur, or
                                part of a growing team, we have the ideal
                                workspace waiting for you.
                            </p>
                        </div>
                    </div>

                    <div class="feature-box fbox-plain fbox-sm">
                        <div class="fbox-icon">
                            <i class="bi-clock"></i>
                        </div>
                        <div class="fbox-content">
                            <h3>Elevate Your Work Environment</h3>
                            <p>
                                Our modern facilities, cutting-edge amenities,
                                and supportive community are tailored to enhance
                                your work experience.
                            </p>
                        </div>
                    </div>

                    <div class="feature-box fbox-plain fbox-sm mb-0">
                        <div class="fbox-icon">
                            <i class="bi-chat-left-text"></i>
                        </div>
                        <div class="fbox-content">
                            <h3>24/7 Access</h3>
                            <p>
                                Our facilities are open 24/7, so you can work
                                whenever you want, however you want.
                            </p>
                        </div>
                    </div>
                </div>

                <div
                    class="col-lg-5 col-md-6 mt-5 mt-md-0"
                    v-if="type === 'trial'"
                >
                    <div class="text-center">
                        <img
                            src="~/assets/images/logo-icon.png"
                            class="img-responsive logo-icon"
                            alt="logo"
                        />
                        <h2 class="ls-0">Try it for Free</h2>
                    </div>
                    <p class="text-muted mb-5">
                        Get a taste of your new workspace with a free trial for
                        1 day. You'll have access to all of our facilities and
                        amenities, so you can experience the benefits of
                        coworking for yourself.
                    </p>
                    <div class="d-flex">
                        <NuxtLink
                            to="/contact"
                            class="button button-rounded button-xlarge d-block flex-fill m-0 text-center text-transform-none fw-semibold ls-0"
                            >Get 1 Day Trial</NuxtLink
                        >
                    </div>
                </div>
                <div class="col-lg-5 col-md-6 mt-5 mt-md-0" v-else>
                    <div class="text-center">
                        <img
                            src="~/assets/images/logo-icon.png"
                            class="img-responsive logo-icon"
                            alt="logo"
                        />
                        <h2 class="ls-0">Take the Next Step</h2>
                    </div>
                    <p class="text-muted mb-5">
                        Ready to take your workspace to the next level? Join our
                        vibrant coworking community today and experience the
                        benefits of a flexible and inspiring environment.
                        <br /><br />From dedicated workstations to
                        state-of-the-art facilities, we have everything you need
                        to thrive.
                    </p>
                    <div class="d-flex">
                        <NuxtLink
                            to="/contact"
                            class="button button-rounded button-warning button-xlarge d-block flex-fill m-0 text-center text-transform-none fw-semibold ls-0"
                            >Become a Member</NuxtLink
                        >
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "CTA",
    props: {
        type: "generic",
    },
};
</script>
<style lang="scss" scoped>
.logo-icon {
    max-height: 100px;
}
</style>
