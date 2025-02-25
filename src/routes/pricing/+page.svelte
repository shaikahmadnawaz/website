<script lang="ts">
    import { FooterNav, MainFooter, PreFooter } from '$lib/components';
    import { DEFAULT_HOST } from '$lib/utils/metadata';

    import { Main } from '$lib/layouts';
    import { TITLE_SUFFIX } from '$routes/titles';
    import ComparePlans from './compare-plans.svelte';
    import Faq from './faq.svelte';
    import BG from './bg.png?enhanced';
    import { PUBLIC_APPWRITE_DASHBOARD } from '$env/static/public';

    const title = 'Pricing' + TITLE_SUFFIX;
    const description = 'Explore our straightforward pricing plans that scale with your project.';
    const ogImage = DEFAULT_HOST + '/images/open-graph/website.png';
</script>

<svelte:head>
    <!-- Titles -->
    <title>{title}</title>
    <meta property="og:title" content={title} />
    <meta name="twitter:title" content={title} />
    <!-- Description -->
    <meta name="description" content={description} />
    <meta property="og:description" content={description} />
    <meta name="twitter:description" content={description} />
    <!-- Image -->
    <meta property="og:image" content={ogImage} />
    <meta property="og:image:width" content="1200" />
    <meta property="og:image:height" content="630" />
    <meta name="twitter:image" content={ogImage} />
    <meta name="twitter:card" content="summary_large_image" />
</svelte:head>

<div
    class="web-location-for-mobile absolute overflow-hidden"
    style:pointer-events="none"
    style:inline-size="100%"
>
    <enhanced:img
        src={BG}
        alt=""
        style="margin-inline:auto; display:block; width: 1369px; height: auto;"
    />
</div>

<Main>
    <div class="web-big-padding-section mt-2">
        <div class="dark pt-10">
            <div class="web-big-padding-section-level-2">
                <section class="container">
                    <div class="web-hero">
                        <h1
                            class="text-display font-aeonik-pro web-u-max-width-700 web-u-opacity-90 web-u-mobile-align-text-center self-center"
                            style="background: linear-gradient(90deg, #F47298 0%, #E4E1E5 61.98%, #E4E4E7 100%);
                                -webkit-background-clip: text; background-clip: text; -webkit-text-fill-color: transparent; padding-block-end:2px;"
                        >
                            Simple, transparent pricing with no surprises
                        </h1>
                    </div>
                </section>
            </div>
            <div class="web-big-padding-section-level-2">
                <section class="container">
                    <div class="web-pricing-cards">
                        <ul class="web-pricing-cards-list">
                            <li>
                                <article
                                    class="web-card is-transparent has-border-gradient h-full"
                                    style="background: linear-gradient(180deg, rgba(255, 255, 255, 0.04) 63.19%, rgba(255, 255, 255, 0.00) 100%);"
                                >
                                    <div class="web-pricing-cards-item">
                                        <header class="web-pricing-cards-header">
                                            <h2 id="starter" class="text-label font-aeonik-pro">Free</h2>
                                            <div
                                                class="text-title font-aeonik-pro text-primary mt-2"
                                            >
                                                $0
                                            </div>
                                            <div class="mt-1">&nbsp;</div>
                                            <p class="text-body mt-4 font-medium h-[5rem]">
                                                For personal hobby projects and students.
                                            </p>
                                            <a
                                                href="{PUBLIC_APPWRITE_DASHBOARD}/register"
                                                class="web-button is-secondary is-full-width mt-8"
                                            >
                                                <span class="text-sub-body font-medium"
                                                    >Start building</span
                                                >
                                            </a>
                                        </header>
                                        <div class="web-pricing-cards-content">
                                            <ul class="web-checked-list-circle">
                                                <li>
                                                    <span>Unlimited projects</span>
                                                </li>
                                                <li><span>Never paused</span></li>
                                                <li><span>10GB bandwidth</span></li>
                                                <li><span>2GB storage</span></li>
                                                <li><span>750K executions</span></li>
                                                <li><span>75K monthly active users</span></li>
                                                <li><span>Community support</span></li>
                                                <li>
                                                    <span>Non-removable Appwrite branding</span>
                                                </li>
                                                <li>
                                                    <span
                                                        >1 Database, 3 Buckets, 5 Functions per
                                                        project</span
                                                    >
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </article>
                            </li>
                            <li>
                                <article
                                    class="web-card is-transparent is-transparent-pink has-border-gradient h-full"
                                    style="background: linear-gradient(180deg, rgba(255, 255, 255, 0.04) 63.19%, rgba(255, 255, 255, 0.00) 100%);"
                                >
                                    <div class="web-pricing-cards-item">
                                        <header class="web-pricing-cards-header">
                                            <header class="flex gap-3">
                                                <h2 id="pro" class="text-label font-aeonik-pro">Pro</h2>
                                                <div class="web-inline-tag is-pink">Popular</div>
                                            </header>
                                            <div
                                                class="text-title font-aeonik-pro text-primary mt-2"
                                            >
                                                $15
                                            </div>
                                            <div class="mt-1">per member/month</div>
                                            <p class="text-body mt-4 font-medium h-[5rem]">
                                                For pro developers and teams that need to scale
                                                their products.
                                            </p>
                                            <a
                                                href="https://cloud.appwrite.io/console?type=createPro"
                                                class="web-button is-full-width mt-8"
                                                target="_blank"
                                                rel="noopener noreferrer"
                                            >
                                                <!-- <span class="text-sub-body font-medium">Start trial</span> -->
                                                <span class="text-sub-body font-medium"
                                                    >Start building</span
                                                >
                                            </a>
                                        </header>
                                        <div class="web-pricing-cards-content">
                                            <p>Everything in Free, plus:</p>
                                            <ul class="web-checked-list-circle">
                                                <li><span>300GB bandwidth</span></li>
                                                <li><span>150GB storage</span></li>
                                                <li><span>3.5M executions</span></li>
                                                <li><span>200K monthly active users</span></li>
                                                <li><span>Organization roles</span></li>
                                                <li><span>Email support</span></li>
                                                <li><span>Add-ons</span></li>
                                                <li>
                                                    <span
                                                        >Unlimited Databases, Buckets, and Functions</span
                                                    >
                                                </li>
                                            </ul>
                                        </div>
                                    </div>
                                </article>
                            </li>
                            <li>
                                <article
                                    class="web-card is-transparent has-border-gradient h-full"
                                    style="background: linear-gradient(180deg, rgba(255, 255, 255, 0.04) 63.19%, rgba(255, 255, 255, 0.00) 100%);"
                                >
                                    <div class="web-pricing-cards-item">
                                        <header class="web-pricing-cards-header">
                                            <h2 id="scale" class="text-label font-aeonik-pro">Scale</h2>
                                            <div
                                                class="text-title font-aeonik-pro text-primary mt-2"
                                            >
                                                $599
                                            </div>
                                            <div class="mt-1">per organization/month</div>
                                            <p class="text-body mt-4 font-medium h-[5rem]">
                                                For scaling teams and agencies that need dedicated
                                                support.
                                            </p>
                                            <button
                                                class="web-button is-secondary is-full-width mt-8"
                                                disabled
                                            >
                                                <span class="text-sub-body font-medium"
                                                    >Coming soon</span
                                                >
                                            </button>
                                        </header>
                                        <div class="web-pricing-cards-content">
                                            <p>Everything in Pro, plus:</p>
                                            <ul class="web-checked-list-circle">
                                                <li><span>Unlimited seats</span></li>
                                                <li><span>SOC-2</span></li>
                                                <li><span>BAA</span></li>
                                                <li><span>Network logs</span></li>
                                                <li><span>28-day log retention</span></li>
                                                <li><span>Custom organization roles</span></li>
                                                <li><span>SSO</span></li>
                                                <li><span>Activity logs</span></li>
                                                <li><span>Priority support</span></li>
                                            </ul>
                                        </div>
                                    </div>
                                </article>
                            </li>
                            <li>
                                <article
                                    class="web-card is-transparent has-border-gradient u-height-100-percent"
                                    style="background: linear-gradient(180deg, rgba(255, 255, 255, 0.04) 63.19%, rgba(255, 255, 255, 0.00) 100%);"
                                >
                                    <div class="web-pricing-cards-item">
                                        <header class="web-pricing-cards-header">
                                            <h2 id="enterprise" class="text-label font-aeonik-pro">Enterprise</h2>
                                            <div
                                                class="text-title font-aeonik-pro text-primary mt-2"
                                            >
                                                Custom
                                            </div>
                                            <div class="mt-1">per organization/month</div>
                                            <p class="text-body mt-4 font-medium h-[5rem]">
                                                For enterprises that need more power and premium
                                                support.
                                            </p>
                                            <a
                                                href="/contact-us/enterprise"
                                                class="web-button is-secondary is-full-width mt-8"
                                                rel="noopener noreferrer"
                                            >
                                                <!-- <span class="web-sub-body-500">Start trial</span> -->
                                                <span class="web-sub-body-500">Contact us</span>
                                            </a>
                                        </header>
                                        <div class="web-pricing-cards-content">
                                            <p>Everything in Scale, plus:</p>
                                            <ul class="web-checked-list-circle">
                                                <li><span>Uptime SLAs</span></li>
                                                <li><span>Designated Success Manager</span></li>
                                                <li><span>24/7 enterprise support</span></li>
                                                <li><span>Private Slack channel</span></li>
                                                <li><span>Volume discounts</span></li>
                                                <li><span>Log drains</span></li>
                                                <li><span>90-day log retention</span></li>
                                                <li><span>Advanced observability</span></li>
                                                <li><span>Bring your own Cloud</span></li>
                                            </ul>
                                        </div>
                                    </div>
                                </article>
                            </li>
                        </ul>
                    </div>

<!--                    <ul class="web-grid-1-1-opt-2 mt-20 gap-8">-->
<!--                        <li>-->
<!--                            <article-->
<!--                                class="web-card is-transparent has-border-gradient min-h-full"-->
<!--                                style="background:rgba(35, 35, 37, 0.90);"-->
<!--                            >-->
<!--                                <header class="flex gap-3">-->
<!--                                    <h3 id="enterprises" class="text-body text-primary font-medium">-->
<!--                                        Enterprises-->
<!--                                    </h3>-->
<!--                                    <div class="web-inline-tag is-pink">Coming Soon</div>-->
<!--                                </header>-->
<!--                                <p class="mt-2">-->
<!--                                    Large scale projects seeking greater performance, collaboration-->
<!--                                    and security.-->
<!--                                </p>-->
<!--                                <a href="/contact-us" class="web-button is-secondary mt-8">-->
<!--                                    <span>Contact us</span>-->
<!--                                </a>-->
<!--                            </article>-->
<!--                        </li>-->
<!--                        <li>-->
<!--                            <article-->
<!--                                class="web-card is-transparent has-border-gradient min-h-full"-->
<!--                                style="background:rgba(35, 35, 37, 0.90);"-->
<!--                            >-->
<!--                                <header class="flex gap-3">-->
<!--                                    <h3-->
<!--                                        id="open-source-teams"-->
<!--                                        class="text-body text-primary font-medium"-->
<!--                                    >-->
<!--                                        Open-source teams-->
<!--                                    </h3>-->
<!--                                </header>-->
<!--                                <p class="mt-2">-->
<!--                                    We support OSS maintainers with a free Pro Plan. Read our-->
<!--                                    announcement blog to find out more.-->
<!--                                </p>-->
<!--                                <a-->
<!--                                    href="/docs/advanced/platform/oss"-->
<!--                                    class="web-button is-secondary mt-8"-->
<!--                                >-->
<!--                                    <span>Learn more</span>-->
<!--                                </a>-->
<!--                            </article>-->
<!--                        </li>-->
<!--                    </ul>-->
                </section>
            </div>
        </div>
        <ComparePlans />

        <div class="dark relative overflow-hidden pt-10">
            <div class="web-big-padding-section-level-2 relative">
                <div class="container relative" style:z-index="10">
                    <section class="web-grid-4-6">
                        <header>
                            <div class="text-display font-aeonik-pro text-primary">FAQ</div>
                        </header>
                        <Faq />
                    </section>
                </div>
            </div>
            <div class="web-big-padding-section-level-2 relative !mb-0">
                <div class="container">
                    <PreFooter />
                    <FooterNav />
                    <MainFooter />
                </div>
            </div>
        </div>
    </div>
</Main>

<style lang="scss">
    .web-card {
        --web-color-border: 240, 4%, 18%;
        --p-card-padding: 1.25rem;
    }
    @media (min-width: 360px) and (max-width: 550px) {
        .web-location-for-mobile {
            inset-block-start: 90px;
        }
    }

    .web-pricing-cards-list {
        gap: 1rem;
        grid-template-columns: repeat(4, 1fr);
    }

    .web-pricing-cards-list .web-main-body-500 {
        height: 78px;
        --p-font-size: unset !important;
        --p-line-height: var(--web-line-height-sm);
    }
</style>
