<template>
    <section class="section">
        <div class="container">
            <header class="section-header">
                <div class="heading-block mb-4 border-bottom-0">
                    <div class="before-heading">Amenities</div>
                    <h2 class="text-transform-none fw-semibold">
                        Everything you need to stay focused
                    </h2>
                </div>
            </header>
            <div class="row">
                <div class="col-12 col-md-6 mb-6" v-for="benefit in list">
                    <div class="mb-2">
                        <i class="fa-2x text-primary" :class="benefit.icon"></i>
                    </div>
                    <h4 v-text="benefit.title"></h4>
                    <p class="lead" v-text="benefit.description"></p>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data() {
        return {
            list: [
                {
                    icon: "fas fa-wifi",
                    title: "Blazing-fast Internet",
                    description:
                        "We provide high-speed internet that allows you to work without any interruptions. Say goodbye to slow loading times and buffering.",
                },
                {
                    icon: "fas fa-chair",
                    title: "Comfortable Seating",
                    description:
                        "Our ergonomic chairs and spacious workspaces are designed to keep you comfortable and productive throughout the day.",
                },
                // {
                //     icon: "fas fa-building",
                //     title: "Dedicated Workspaces and Private Offices",
                //     description:
                //         "We offer a range of workspace options to meet your needs, from shared workspaces to private offices that you can make your own.",
                // },
                {
                    icon: "fas fa-users",
                    title: "High-quality Conference Room",
                    description:
                        "Our conference room is perfect for meetings, presentations, and workshops, with the latest technology and space for up to 20 people.",
                },
                {
                    icon: "fas fa-print",
                    title: "Printing Facilities",
                    description:
                        "Need to print important documents or presentations? Printing facilities are available on-site. No more searching for print shops - get everything done under one roof.",
                },
                {
                    icon: "fas fa-utensils",
                    title: "Fully Equipped Kitchen",
                    description:
                        "Our kitchen is stocked with everything you need to fuel your workday, including coffee, tea, snacks, and more.",
                },
                {
                    icon: "fas fa-mug-hot",
                    title: "Free Tea/Coffee",
                    description:
                        "Enjoy unlimited complimentary tea and coffee to help fuel your workday. Our kitchen is fully stocked with everything you need to keep you energized and focused.",
                },
                {
                    icon: "fas fa-envelope",
                    title: "Reception & Mail Handling",
                    description:
                        "Our receptionist is always available to greet your clients and handle your mail, so you can focus on growing your business.",
                },
                {
                    icon: "fas fa-gamepad",
                    title: "Gaming & Relaxing Room",
                    description:
                        "Take a break from work and unwind in our gaming room or relax in our comfortable lounge area, complete with a massage chair.",
                },
                {
                    icon: "fas fa-shield-alt",
                    title: "24/7 Security",
                    description:
                        "Our premises are monitored by 24/7 security cameras and our front desk is staffed during business hours to ensure that our members feel safe and secure.",
                },
                {
                    icon: "fas fa-lock",
                    title: "Personal Lockers",
                    description:
                        "Keep your belongings safe and secure in your own personal locker. Enjoy peace of mind knowing that your belongings are safe and easily accessible.",
                },
                {
                    icon: "fas fa-snowflake",
                    title: "Air Conditioning",
                    description:
                        "Stay comfortable and focused in our air-conditioned coworking space. Our temperature-controlled environment ensures that you can work in comfort, no matter the weather outside.",
                },
                {
                    icon: "fas fa-bolt",
                    title: "Uninterrupted Power",
                    description:
                        "Stay connected and productive even during power outages. Our coworking space is equipped with a backup power supply, ensuring that you have uninterrupted access to electricity.",
                },
            ],
        };
    },
};
</script>
