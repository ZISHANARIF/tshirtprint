/* **********************show product section code*************** */
.services-section {
    background: var(--bg2-color);
}

.service-card {
    background-color: var(--bg1-color);
    /* border-radius: var(--radius); */
    box-shadow: 0 5px 25px rgba(0, 0, 0, 0.08);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    height: 100%;
    overflow: hidden;
    text-decoration: none;
    display: flex;
    flex-direction: column;
    color: inherit;
}

.service-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.12);
}

.image-wrapper {
    position: relative;
    overflow: hidden;

}

.card-image {
    aspect-ratio: 1/1;
    width: 100%;
    height: auto;
    /* Fixed height for consistent card appearance */
    object-fit: cover;
    display: block;
    transition: transform 0.5s ease;
}

.image-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: var(--secondary-color);
    opacity: 0.4;
    transform: translateY(-100%);
    /* Start off-screen above */
    transition: transform 0.5s ease;
    display: flex;
    align-items: center;
    justify-content: center;
}

.service-card:hover .image-overlay {
    transform: translateY(0);
}

.card-body {
    padding: 1rem;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
}

.card-body .leadsuresubheading:hover {
    cursor: pointer;
}

.product-item .product-title {
    color: #1A2953;
    font-size: 20px;
    font-weight: 700;
    text-transform: uppercase;
    margin-bottom: 15px;
}


/* ********************video section code****************** */
.video-embed-section {
    background-color: var(--bg1-color);
}

.video-frame {
    box-shadow: 15px 15px 0px 0 var(--primary-color);

    background-color: var(--bg1-color);
    line-height: 0;
}

.video-frame .ratio iframe {
    display: block;
}


/* ******************our products section*************************** */
.projects-section {
    background-color: var(--bg2-color);
}



/*--------------------------------
        # Custom Bootstrap Nav Tabs
        --------------------------------*/
.project-tabs {
    border-bottom: none;
    margin-bottom: 30px;
}

.project-tabs .nav-item {
    margin: 0 5px;
}

.project-tabs .nav-link {
    border: none;
    color: var(--para-color);
    font-weight: 600;
    text-transform: uppercase;
    font-size: 14px;
    padding: 10px 15px;
    transition: all 0.3s ease;
}

.project-tabs .nav-link:hover {
    color: var(--hover-color1);
}

.project-tabs .nav-link.active {
    color: var(--heading-color);
    background-color: transparent;
    font-size: 16px;
    border: none;
}


/* ************************working process section code************************* */

.working-process-section {
    /* Using a dark, textured background image as requested */
    background-image: url('https://templates.thememodern.com/theratio/images/bg//bg2-process.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
}




/* Individual Step Styling */
.process-step {
    position: relative;
    padding-top: 40px;
    /* For mobile stacking */
    margin-bottom: 30px;
}

.process-step .step-number {
    position: absolute;
    top: -37px;
    left: 39%;
    transform: translateX(-50%);
    font-size: 82px;
    font-weight: 700;

    color: rgba(255, 255, 255, 0.1);
    z-index: 1;
}

.process-step .step-icon-wrapper {
    width: 125px;
    height: 125px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 auto 20px auto;
    /* Inactive state (default) */
    background-color: #000000;
    color: var(--light-color);
    border: 2px solid var(--white);
    /* Subtle border */
    font-size: 36px;
    position: relative;
    z-index: 2;
    transition: all 0.3s ease;
}

/* Active state styling */
.process-step.active .step-icon-wrapper {
    background-color: var(--bg1-color);
    color: var(--white);
    border-color: var(--bg1-color);
}

.process-step .step-title {
    color: var(--light-color);
    font-size: var(--heading-size);
    font-weight: 600;
    margin-bottom: 10px;
}

.process-step .step-icon-wrapper:hover {
    background-color: var(--bg1-color);
    color: var(--white);
}



/* Bottom Description */
.working-process-section .section-description {
    color: var(--dark-text);
    font-size: var(--para-size);
    line-height: 1.7;

    margin-top: 20px;
}


/* ***************advantges section code********************* */


.advantages-section {
    background-color: var(--bg2-color);
    position: relative;
    overflow: hidden;
}

.advantages-section::before,
.advantages-section::after {
    content: '';
    position: absolute;
    width: 400px;
    height: 100%;
    /* URL-encoded SVG for a simple vector grid */
    background-image: url('https://media.istockphoto.com/id/1913232085/vector/simple-shower-black-line-icon.jpg?s=612x612&w=0&k=20&c=5CFMhG7l3sK-SQFU8crsnXvHq6xvkm25nbaRwnDt_rk=');
    background-repeat: no-repeat;
    background-color: transparent;
    /* Very faint */
    opacity: 0.1;
    z-index: 0;
    /* animation: bounceY 4s 
ease-in-out infinite; */
}

.advantages-section::before {
    top: -80px;
    left: 50px;
    transform: rotate(-28deg);

}

/* Position for bottom-right vector */
.advantages-section::after {
    bottom: -90px;
    right: 100px;
    transform: rotate(125deg);

}

/* Ensure content stays above the backgrounds */
.advantages-section .container-fluid {
    position: relative;
    z-index: 2;
}


/* Central Image */
.advantage-image {
    border-radius: 50%;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    width: 100%;
    aspect-ratio: 1 / 1;
    object-fit: cover;
}


/* ***************** image + text  content section code****************** */

.why-choose-us-section {

    background-color: var(--bg1-color);
    overflow: hidden;
}

/* Section Header */
.why-choose-us-section .section-subtitle {

    color: #e11d2a;
    font-size: 14px;
    font-weight: 600;
    margin-bottom: 10px;
}



/* Map Image Wrapper */
.map-image-wrapper {
    aspect-ratio: 1/1;
    width: 100%;
    height: auto;




/* ***************************SEO SECTION CODE****************** */
.section-highlight {
    background: var(--bg2-color);
}

.feature-copy {
    position: relative;
    color: var(--para-color);
    font-size: 14px;
    line-height: 1.6;
    background: var(--background2-color);
    padding: 18px 10px;
    overflow: hidden;
}

/* Collapse content initially */
.feature-copy .seo-content61 {
    max-height: 315px;
    /* collapsed */
    overflow: hidden;
    transition: max-height 0.5s ease;
}

.scrollcard {
    width: 100%;
}

.scrollcard img {
    aspect-ratio: 1/1;
    box-shadow: 15px 15px 0px 0 var(--primary-color);
    object-fit: cover;
}



/* Hidden checkbox */
.read-more-toggle {
    display: none;
}

/* Expand when checked */
.read-more-toggle:checked~.seo-content61 {
    overflow-y: auto;
    scrollbar-width: thin;
}

/* Read more button */
.read-more-btn {
    display: block;
    text-align: left;
    /* button floats right side */
    margin-top: 10px;
    color: var(--btn-color);
    font-size: var(--heading-size);
    cursor: pointer;
    transition: color 0.3s;
}


/* Toggle text dynamically */
.read-more-btn::after {
    content: "Show More...";
    color: var(--primary-color);
    font-size: var(--para-size);
}

.read-more-btn:hover::after {
    color: var(--secondary-color);
}

.read-more-btn:hover::before {
    color: var(--primary-color);
}

.read-more-toggle:checked~.read-more-btn::after {
    content: "Show Less...";
    color: var(--hover-color);
    font-size: var(--para-size);

}




/* faq section code******************************** */

.faq-container {

    background-image: url('https://templates.thememodern.com/theratio/images/bg/bg2-home3.jpg');
}



.left-section {

    padding: 10px;

    min-height: 1px !important;


    transition: min-height 0.3s ease;
}


.faq-title {
    font-size: var(--title-size);
    font-weight: 600;
    color: var(--heading-color);
    margin-bottom: 10px;
    line-height: 1.2;
}






.right-section {
    flex: 1;
    padding: 40px;
}

.faq-item {

    position: relative;
    margin-bottom: 10px;
    border-left: 3px solid var(--primary-color);
    box-shadow: 0 1px 0 rgba(0, 0, 0, .05);

}

.faq-item:last-child {
    border-bottom: none;
}

.faq-question {
    background: var(--bg1-color);
    /* background-color: transparent; */
    border: none;
    padding: 10px 40px 18px 10px;
    font-size: var(--para-size);
    font-weight: 600;
    color: var(--heading-color);
    cursor: pointer;
    width: 100%;
    text-align: left;
    position: relative;
    transition: all 0.3s ease;

}



.faq-question::after {
    content: '\f107';
    font-family: 'Font Awesome 6 Free';
    font-weight: 900;
    position: absolute;
    right: 3%;
    top: 50%;
    transform: translateY(-50%) rotate(-90deg);
    transition: transform 0.3s ease;
    font-size: 16px;
    color: var(--btn-color);
}

.faq-answer {
    max-height: 0;
    overflow: hidden;
    transition: 0.3s ease;
    padding: 0;
    color: var(--para-color);
    font-size: var(--para-size);
    line-height: 1.6;
    box-shadow: 5px 5px 27px rgba(0, 0, 0, 0.3);
}


/* Active states */
.faq-item.active .faq-question::after {
    transform: translateY(-50%) rotate(0deg);
}

.faq-item.active .faq-answer {
    max-height: 200px;
    padding: 10px;

}



@media (max-width: 768px) {
    .faq-wrapper {
        flex-direction: column;
    }



    .right-section {
        padding: 10px;
    }


}


.iti--separate-dial-code .iti__selected-flag {

    height: 40px;
}

.lable {
    color: red;
}

/* --- Right Side: Enquiry Form --- */
.enquiry-form-wrapper {
    background-color: var(--bg1-color);
    color: var(--heading-color);
    padding: 25px;
    border-radius: var(--radius);
}

@media (max-width: 991.98px) {
    .enquiry-form-wrapper {
        margin-top: 3rem;
    }
}

.enquiry-form-wrapper .form-heading {
    font-size: var(--heading2-size);
    font-weight: 600;
    color: var(--primary-color);
}

.enquiry-form-wrapper .form-subheading {
    color: var(--para-color);
    margin-bottom: 1rem;
}

.form-control,
.input-group-text {
    border: 1px solid var(--border-light);
    padding: 0.85rem 1rem;
    transition: border-color 0.3s ease;
}

.form-control:focus {
    border-color: var(--secondary-color);
    box-shadow: 0 0 0 0.2rem rgba(229, 109, 72, 0.25);
}



/* *****************blog section code***************************** */

.latest-news-section {

    background-color: var(--bg1-color);

}



.latest-news-section .title-separator {
    /* Dotted line from screenshot */
    display: inline-block;
    width: 50px;
    height: 2px;
    border-top: 2px dotted #aaa;
    margin-bottom: 50px;
}


.blog-card {
    display: block;
    border: 1px solid var(--border-light);
    border-radius: 1px;
    transition: all 0.3s ease;
    height: 100%;
}

.blog-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
}

/* Wrapper to position the category tag */
.blog-card .card-img-wrapper {
    position: relative;
}

.blog-card .card-img-top {
    border-radius: 0;
    aspect-ratio: 4 / 3;
    object-fit: cover;
}

.blog-card .card-category-tag {
    position: absolute;
    bottom: 15px;
    left: 15px;
    background-color: var(--white);
    color: var(--light-color);
    padding: 4px 10px;
    font-size: var(--para-size);
    font-weight: 500;
    text-transform: uppercase;
}

/* Card body styles */
.blog-card .card-body {
    padding: 25px;
}

.blog-card .card-meta {
    color: var(--secondary-color);
    font-size: var(--para-size);
    text-transform: uppercase;
    margin-bottom: 10px;
}



/* ***************************our partner section code****************************** */
.partners-section {
    background-color: var(--bg2-color);
}

.partner-heading {
    font-size: var(--title-size);
    color: var(--heading-color);
    font-weight: 600;
}

.partner-para {
    color: var(--para-color);
    font-size: var(--para-size);
}

/* 2. Swiper Container & Slide Styling */
.swiper {
    width: 100%;
    height: 100%;
}

.swiper-slide {
    text-align: center;
    font-size: 18px;
    background: transparent;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem 0;
}


.swiper-slide img {
    display: block;
    width: 150px;
    height: auto;
    object-fit: contain;


    transition: filter 0.3s ease, opacity 0.3s ease;
}

.swiper-slide:hover img {
    filter: grayscale(0%);
    opacity: 1;
}

/* Optional: Style for the pagination dots */
.swiper-pagination-bullet-active {
    background-color: var(--secondary-color);
}

.swiper-horizontal>.swiper-pagination-bullets,
.swiper-pagination-bullets.swiper-pagination-horizontal {
    bottom: -6px;


}



/* **********************our history section code*********************** */

.history-section {
    overflow: hidden;
    background-color: var(--bg2-color);
}


/*--------------------------------
        # Swiper Timeline (Years)
        --------------------------------*/
.history-timeline-swiper {
    width: 100%;
    height: 100px;
    padding: 10px 0;
    position: relative;
}

.history-timeline-swiper .swiper-slide {

    color: var(--para-color);
    font-size: var(--heading3-size);
    font-weight: 600;
    text-align: center;
    cursor: pointer;
    transition: all 0.3s ease;
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0.5;
}

.history-timeline-swiper .swiper-slide-active {
    /* Styles for the active (centered) slide */
    color: var(--heading-color);
    font-size: var(--large-text);
    font-weight: 700;
    transform: scale(1.1);
}

/* Triangle connector */
.timeline-connector {
    width: 0;
    height: 0;
    border-left: 20px solid transparent;
    border-right: 20px solid transparent;
    /* Light grey border color */
    border-top: 20px solid var(--secondary-color);
    /* Positioned just below the slider */
    margin: 10px auto 10px auto;

    position: relative;
    z-index: 10;
}

/*--------------------------------
        # History Content Area
        --------------------------------*/
.history-content-wrapper {
    padding: 56px 1px;
    background-color: var(--bg1-color);
}

.history-content-item {
    /* Hide all content items by default */
    display: none;
    animation: fadeIn 0.5s ease;
}

.history-content-item.active {
    /* Show the active one */
    display: block;
}


.history-content-item .content-text {
    color: #777;
    font-size: 16px;
    line-height: 1.7;
    max-width: 700px;
    margin: 0 auto;
}

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateX(10px);
    }

    to {
        opacity: 1;
        transform: translateX(0);
    }
}

/* ***********************matrix section code************************** */
.stats-section {

    position: relative;
    background: url('https://templates.thememodern.com/theratio/images/bg/bg2-aboutus.jpg') no-repeat center center;

    background-size: cover;
    background-attachment: fixed;
    /* Creates a nice parallax effect */

}

.stat-item {
    text-align: center;
}

@media (max-width: 767.98px) {
    .stat-item {
        margin-bottom: 2.5rem;
    }
}

.stat-number {
    font-size: 3rem;
    font-weight: 600;
    color: var(--para-color);
    margin-bottom: 0.5rem;
}

.stat-label {
    font-size: var(--heading-size);
    color: var(--heading-color);
}


/* *********************product section code********************* */

.speedproducts-section {
    background-color: var(--bg2-color);
}

.speedproducts-card {
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    border-radius: var(--radius);
    background-color: var(--bg1-color);
}

.card-footer {
    background-color: var(--bg1-color);
}

.speedproducts-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.1) !important;
}

.speedproducts-img-ratio {
    position: relative;
    width: 100%;
    padding-top: 100%;
    overflow: hidden;
}

.speedproducts-img-ratio img {
    aspect-ratio: 1 / 1;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: auto;
    object-fit: cover;
}

.speedproducts-img-container {
    overflow: hidden;
}

.speedproducts-img-top {
    transition: transform 0.4s ease;
}

.speedproducts-card:hover .speedproducts-img-top {
    transform: scale(1.05);
}

.speedproducts-link {
    color: var(--btn-color2);
    font-size: var(--para-size);
}

.speedproducts-link svg {
    color: var(--primary-color);
}

.speedproducts-link:hover {
    color: var(--hover-color2);
}

.speedproducts-title-link {
    text-decoration: none;
}

.speedproducts-title:hover {
    color: var(--hover-color2);
}



/* *********************category page section code************************** */
.lab-section {
    background-color: var(--bg2-color);
}

.content-section {
    width: 100%;
}

.left-content-wrapper {
    float: right;
    max-width: 400px;
    width: 100%;
    margin-left: 1.5rem;
    margin-bottom: 1rem;
    border: 1px solid var(--secondary-color);
}

.image-container {
    aspect-ratio: 1/1;
    position: relative;
    width: 100%;
    padding-bottom: 100%;
    overflow: hidden;
    border-radius: 0;
    margin-bottom: 20px;
}

.image-container img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.product-description p,
.product-description li,
.product-description ul {
    line-height: 1.6;
    text-align: justify;
    margin-bottom: 6px;
}
.button-container {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    justify-content: space-evenly;
    margin-bottom: 20px;
}


/* ********************meet our team section code************************ */
.team-section {

            background-color:var(--bg1-color);
        }


        .team-card {

            border: none;
            border-radius: 8px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.09);
            height: 100%;
            transition: all 0.3s ease;
        }

        .team-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .team-card .card-body {
            text-align: center;
            padding: 10px;
        }

        .team-card .team-image {
            aspect-ratio: 1 / 1;
            width: 100%;
            height: auto;
            object-fit: cover;
            /* border: 4px solid #ffffff;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); */
            margin-bottom: 20px;
        }



        /* *******************contact us section code**************************** */
.contact-section-overlap {
            
            background-color: var(--bg2-color);
          
        }
        .get-in-touch-wrapper{
            background-color: var(--bg1-color);
            padding: 30px;
        }
    
        .contact-details-wrapper {
            background-color: var(--footer-color);
            padding: 20px 40px;
            margin-top: 0;
            margin-bottom: 0;
            position: relative;
            z-index: 10;
        }
        .info-block {
            margin-bottom: 25px;
        }
       
        .contact-box a{
            text-decoration: none;

        }
        .contact-box a:hover{
            text-decoration: underline;
            cursor: pointer;
        }


                /*************************** privacy policy content********************** */

.privacy-container {


    background-color: var(--bg2-color);
}

.heading-1 {
    

    font-size: var(--heading2-size);

    color: var(--heading-color);

    margin-bottom: 20px;

    font-weight: 600;
}

.privacy-container a {
    font-size: var(--para-size);

    color: var(--primary-color);
}
.privacy-box{
    padding: 20px;
    background: var(--bg1-color);
}

/* ****************market area section code ************** */

/* Section Wrapper */
.market-area {
    background: var(--bg2-color)
}

/* Heading */
.Marektheading {
    text-align: center;
    margin-bottom: 30px;
}

.Marektheading {
    font-size: var(--title-size);
    font-weight: 600;
    color: var(--heading-color);
}



/* Sub-headings (States & Cities titles) */
.market-area h2 {
    font-size: var(--heading2-size);
    font-weight: 600;
    margin: 30px 0 15px;
    color: var(--heading-color);
    border-left: 5px solid var(--primary-color);
    padding-left: 10px;
}

/* Market Cards */
.marketcard {
    display: block;
    text-align: center;
    padding: 12px 10px;
    
    border-radius: var(--radius);
    background: var(--bg1-color);
    box-shadow: 0 4px 10px rgba(59, 59, 59, 0.1);

    font-size: 16px;
    /* font-weight: 500; */
    color: var(--secondary-color);
    text-decoration: none;
    transition: all 0.3s ease;
}

/* Hover effect */
.marketcard:hover {
    /* background: var(--); */
    color: var(--hover-color1);

    transform: translateY(-3px);
    background-color: var(--secondary-color);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}








        /* ************************BLOG DETIL PAGE SECTION************************************ */
.blog-section105{
    background-color: var(--bg2-color);
}

.main-content105 {
            background-color: var(--bg1-color);
            padding: 2rem;
            border: 1px solid var(--border-color);
        }
        
        @media (max-width: 767.98px) {
            .main-content105 {
                padding: 1.5rem;
            }
        }

        .blog-title-wrapper105 {
            display: flex;
            align-items: flex-start;
            gap: 0.75rem;
            margin-bottom: 10px;
        }
        
        .blog-title-wrapper105 .title-icon105 {
            flex-shrink: 0;
            width: 24px;
            height: 24px;
            margin-top: 0.5rem;
        }

        .blog-title105 {
            font-size: 2.25rem;
            font-weight: 900;
            color: var(--heading-color);
            line-height: 1.3;
        }

        .blog-image105 {
            width: 100%;
            aspect-ratio: 16 / 9;
            object-fit: cover;
            border-radius:var(--radius) ;
            margin-bottom: 2rem;
        }
       .post-dateX {
    font-size: var(--para-size);
    color: var(--para-color);
    font-weight: 600;
}
            /* --- NEW/MODIFIED STYLE FOR THE DATE --- */
        .blog-meta105 {
            /* margin-top: 1rem;
            margin-bottom: 1rem; */
            color: var(--primary-color);
            font-size: var(--para-size);
            display: flex;
            font-weight: 700;
            align-items: center;
            gap: 0.5rem;
        }
        
        .blog-meta105 .meta-icon {
            width: 16px;
            height: 16px;
        }
        

      

        /* --- Sidebar --- */
        .sidebar105 .widget105 {
            background-color: var(--secondary-color);
            padding: 1.5rem;
            border: 1px solid var(--bg2-color);
        }
        
        .widget-title105 {
            font-size: var(--heading-size);
            font-weight: 600;
            color: var(--light-color);
            padding-bottom: 0.75rem;
           margin-bottom: 10px;
            border-bottom: 1px solid var(--primary-color);
        }

        .related-blogs-list105 {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        
        .related-post-item105 {
            display: flex;
            gap: 1rem;
        }
        
        .related-post-item105:not(:last-child) {
            margin-bottom: 1rem;
        }

        .related-post-item105 img {
            aspect-ratio: 4 / 3;
    width: 100%;
    height: auto;
            border-radius: var(--radius)
        }

        .related-post-item105 .post-title105 {
            font-weight: 700;
            line-height: 1.6;
            font-size: var(--para-size);
            
        }

        .related-post-item105 .post-title105 a {
            text-decoration: none;
            color: var(--heading-color);
            transition: color 0.3s ease;
        }
        
        .related-post-item105 .post-title105 a:hover {
            color: var(--hover-color1);
        }




        /* **************************** NEW FAQ SECTION CODE************************************  */


.faq-section62{
            background-color: var(--bg1-color);
            padding: 6px 0px 56px 0px;
        }
        
        /* --- Bootstrap Nav Tabs Styling --- */
        .faq-nav-tabs {
            border-bottom: none;
            justify-content: center;
        }
        .nav-link{
            margin-bottom: 5px;
        }
        .faq-nav-tabs .nav-link {
            border: none;
            color: var(--white);
            background-color: var(--primary-color);
            border-radius: var(--radius);
            padding: 0.5rem 1.5rem;
            font-weight: 500;
            margin: 0.5rem;
            transition: all 0.2s ease-in-out;
        }
        .faq-nav-tabs .nav-link:hover{
            background: var(--hover-color1);
        }
        .faq-nav-tabs .nav-link.active {
            color: var(--white);
            background-color: var(--hover-color1);
        }
        
        
        .custom-accordion-item {
           
            
            border-radius: 0.75rem;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
            margin-bottom: 1rem;
            padding: 1.25rem 1.5rem;
        }
        .custom-accordion-question {
            font-weight: 500;
            color: var(--heading-color);
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .custom-accordion-answer {
            max-height: 0;
            overflow: hidden;
            color: var(--para-color);
            transition: max-height 0.3s ease-in-out, padding-top 0.3s ease-in-out;
        }
        
        /* Active State (Toggled by JavaScript) */
        .custom-accordion-item.active .custom-accordion-question {
            font-weight: 600;
            color: var(--primary-color);
        }
        .custom-accordion-item.active .custom-accordion-answer {
            max-height: 200px;
            padding-top: 0.75rem;
            font-size: var(--para-size);

        }
        
        /* Plus/Minus Icon */
        .icon-toggle {
           width: 1.75rem;
    height: 1.75rem;
    background-color:var(--primary-color);  
    color: var(--white);           
    font-weight: bold;
    font-size: 1rem;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: var(--radius); 
    cursor: pointer;
        }
        .custom-accordion-item.active .icon-toggle {
              background-color: var(--hover-color1); 
    background-image: none; 
              }

              .custom-accordion-item.active .icon-toggle::after {
    content: "−";  /* minus sign */
}

/* Default state: show plus */
.icon-toggle::after {
    content: "+";  /* plus sign */
}




/* ********************certifcation section code***************************** */

.certifications-section {
    background-color: var(--bg2-color);
}

.certificate-card {
    display: block;
    text-decoration: none;

    border-radius: var(--radius);
    padding: 0.2rem;
    background-color: var(--border-light);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
      transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
            position: relative; /* Required for the overlay */
            overflow: hidden; 
}

.certificate-card img {
    width: 100%;
    height: auto;
    aspect-ratio: 1/1;
    object-fit: cover;

}

.certificate-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
}

        .card-hover-title {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            background: linear-gradient(to top, rgba(10, 10, 10, 0.9), transparent);
            color: var(--light-color);
            padding: 2rem 1rem 1rem 1rem;
            text-align: center;
            opacity: 0;
            transform: translateY(100%);
            transition: opacity 0.3s ease, transform 0.3s ease;
        }

        .card-hover-title .galleryhead {
            margin: 0;
            font-size: var(--heading-size);
            color: var(--light-color);
            font-weight: 600;
        }
        
        /* Show the title on hover */
        .certificate-card:hover .card-hover-title {
            opacity: 1;
            transform: translateY(0);
        }
    

        /* *****************************siteMap Section code**************************** */
.sitemap-section {
    
    background: var(--bg2-color);

}
.sitemapbox{
    padding: 20px;
    background: var(--bg1-color);
}
.sitemap-section .sitempheading {
    font-size: var(--heading2-size);
    font-weight: 600;
    margin-bottom: 20px;
    border-bottom: 3px solid var(--secondary-color);
    display: inline-block;
    padding-bottom: 5px;
    color: var(--header-color);
}

/* Root UL */
.sitemapcon {
    list-style: none;
    padding-left: 0;
    margin: 0;
    font-size: var(--para-size);
}

/* Parent LI */
.sitemapcon>li {
    position: relative;
    margin: 10px 0;
    padding-left: 20px;
}

/* Add vertical line before items */
.sitemapcon>li::before {
    content: "";
    position: absolute;
    top: 0;
    left: 8px;
    bottom: 0;
    border-left: 2px solid var(--primary-color);
}

/* Horizontal line for each item */
.sitemapcon>li::after {
    content: "";
    position: absolute;
    top: 12px;
    left: 8px;
    width: 10px;
    border-top: 2px solid var(--primary-color);
}

/* Links */
.sitemapcon a {
    text-decoration: none;
    color: var(--para-color);
    font-size: var(--para-size);
    transition: color 0.2s;
}

.sitemapcon a:hover {
    color: var(--hover-color1);
    font-weight: 600;
}

/* Subcategories */
.sitemapsubcat {
    list-style: none;
    margin: 5px 0 5px 20px;
    padding-left: 15px;
    border-left: 2px solid var(--secondary-color);
}

.sitemapsubcat li {
    position: relative;
    margin: 10px 0;
    padding-left: 15px;
}

.sitemapsubcat li::before {
    content: "";
    position: absolute;
    top: 12px;
    left: -15px;
    width: 15px;
    border-top: 2px solid var(--secondary-color);
}

/* Responsive adjustments */
@media (max-width: 767px) {
    .sitemap-section {
        padding: 20px 10px;
    }

    .sitemap-section .you_may {
        font-size: 16px;
    }

    .sitemapcon {
        font-size: 13px;
    }
}

