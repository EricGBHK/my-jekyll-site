<!DOCTYPE html>
<html lang=en>
    <head>
        <meta charset=utf-8>
        <meta content="Tom MacWright" name=author>
        <meta content=#fff name=theme-color>
        <meta content="" name=twitter:title>
        <meta content="" property=og:title>
        <meta content=https://macwright.com/ property=og:url>
        <meta content=@tmcw@mastodon.social name=fediverse:creator>
        <meta content="The blog, projects, and assorted output of Tom MacWright" name=description>
        <meta content="The blog, projects, and assorted output of Tom MacWright" name=twitter:description>
        <meta content="The blog, projects, and assorted output of Tom MacWright" name=og:description>
        <meta content="width=device-width,initial-scale=1" name=viewport>
        <meta content=macwright.com property=og:site_name>
        <meta content=tom@macwright.com property=og:email>
        <meta content="Jekyll v4.4.1" name=generator>
        <meta content=website property=og:type>
        <meta content=1458271 property=twitter:account_id>
        <script type=application/ld+json>
            {
                "@context": "http://schema.org",
                "@type": "CreativeWork",
                "author": {
                    "@type": "Person",
                    "name": "Tom MacWright"
                }
            }</script>
        <link href=https://macwright.com/rss.xml rel=alternate type=application/rss+xml title=macwright.com>
        <link href=https://macwright.com/atom.xml rel=alternate type=application/atom+xml title=macwright.com>
        <link href=/css/favicon.png rel=icon type=image/x-icon>
        <style>
            :root {
                --mono-font: "Berkeley Mono", "JetBrains Mono", "Fira Code", San Francisco Mono, Monaco, "Consolas", "Lucida Console", "DejaVu Sans Mono", "Bitstream Vera Sans Mono", monospace;
                --sans-font: -apple-system, BlinkMacSystemFont, "avenir next", avenir, helvetica, "helvetica neue", ubuntu, roboto, noto, "segoe ui", arial, sans-serif
            }

            a.front-page-title {
                display: block;
                font-weight: 900;
                padding-bottom: 5px;
                text-decoration: none
            }

            a,a.front-page-title:hover {
                text-decoration: underline
            }

            div.front-page-images {
                display: grid;
                grid-template-columns: repeat(auto-fit,minmax(80px,1fr));
                grid-gap: 5px
            }

            div.front-page-images>div {
                display: flex;
                align-items: center;
                line-height: 0
            }

            div.front-page-images>div img {
                width: 100%;
                aspect-ratio: 1/1;
                object-fit: cover
            }

            .star {
                width: 13px;
                height: 12px;
                display: inline-block;
                background: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTMiIGhlaWdodD0iMTIiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTYuMzA5IDkuMjJMMi40MDkgMTJsMS40NC00LjU2N0wwIDQuNTgzbDQuNzg4LS4wNDJMNi4zMDggMCA3LjgzIDQuNTRsNC43ODkuMDQ0LTMuODUgMi44NDlMMTAuMjA5IDEyeiIgZmlsbC1ydWxlPSJldmVub2RkIi8+PC9zdmc+)
            }

            body {
                color: #111;
                margin: 0 auto;
                -webkit-font-smoothing: antialiased;
                text-rendering: optimizeLegibility;
                line-height: 1.6;
                font-size: 1rem;
                font-family: var(--sans-font)
            }

            .only-print {
                display: none
            }

            .body img {
                width: 100%;
                height: auto;
                max-width: 640px
            }

            a {
                color: #000;
                text-decoration-skip-ink: auto
            }

            a:visited {
                color: #333
            }

            ul {
                margin: 1rem 0
            }

            ul ul {
                margin: 0
            }

            br {
                line-height: 1em
            }

            h2 {
                margin-bottom: .5rem;
                line-height: 1.25;
                font-weight: 600;
                font-size: 1.5rem;
                letter-spacing: .009em
            }

            .limiter {
                max-width: 640px;
                padding-left: 20px;
                padding-right: 20px;
                margin-left: auto;
                margin-right: auto
            }

            .pad2y {
                padding-top: 20px;
                padding-bottom: 20px
            }

            .books,.writing {
                display: grid;
                grid-column-gap: 5px;
                grid-row-gap: 5px
            }

            .writing {
                grid-template-columns: 1fr min-content
            }

            .books {
                grid-template-columns: 1fr .75fr min-content 70px
            }

            .books a,.writing a {
                font-weight: 500;
                letter-spacing: -.015em
            }

            .books>div,.writing>div {
                white-space: nowrap;
                overflow: hidden;
                text-overflow: ellipsis
            }

            .books time,.writing time {
                padding-right: .25em;
                color: #333;
                font-variant-numeric: tabular-nums;
                letter-spacing: -.012em;
                white-space: pre
            }

            .micro>div {
                margin-bottom: 20px;
                border: 1px solid #000;
                border-radius: 2px
            }

            .body li,.micro li {
                list-style-type: "-  "
            }

            .micro>div>.body {
                background-color: #f9f9f9;
                padding: 20px
            }

            .micro>div>div:first-child {
                padding: 10px 20px;
                border-bottom: 1px solid #000;
                display: flex;
                justify-content: space-between
            }

            .micro>div>div:first-child>a {
                font-weight: 700
            }

            .micro>div>div:first-child>h2 {
                font-size: inherit;
                margin: 0;
                line-height: inherit
            }

            .micro>div>div:first-child>time {
                white-space: pre
            }

            .micro a {
                color: #00f
            }

            @media screen and (max-width: 640px) {
                div.front-page-images>div:nth-child(4) {
                    display:none
                }

                .limiter {
                    width: auto
                }

                .books,.writing {
                    grid-template-columns: 1fr;
                    grid-row-gap: 0
                }

                .books div,.writing div {
                    white-space: normal
                }

                .books div:nth-child(4n),.writing time {
                    padding-bottom: 20px
                }
            }

            @media screen and (min-width: 640px) {
                .nu a {
                    text-decoration:none
                }

                .nu a:hover {
                    text-decoration: underline
                }
            }

            @media screen and (max-width: 1024px) {
                .header-wrap {
                    border-bottom:1px solid #000;
                    padding-bottom: 20px
                }
            }

            @media screen and (min-width: 1025px) {
                .header {
                    position:absolute;
                    top: 42px;
                    right: 50%;
                    margin-right: 340px!important;
                    letter-spacing: -.009em
                }
            }

            @media print {
                .no-print {
                    display: none
                }

                .only-print {
                    display: block
                }

                body {
                    margin: 0
                }

                .limiter {
                    max-width: 100%!important;
                    margin: 0!important;
                    padding: 0!important
                }
            }
        </style>
        <title>macwright.com</title>
        <link href=https://bsky.app/profile/macwright.com rel=me>
        <link href=https://mastodon.social/@tmcw rel=me>
        <link href=https://github.com/tmcw rel=me>
        <link href=mailto:tom+2024@macwright.com rel=me>
        <link href=https://macwright.com/ rel=canonical>
    </head>
    <body class=post>
        <div class=pad2y style=position:relative>
            <div class=only-print>
                <h2>
                    <a href=/>Tom MacWright</a>
                </h2>
                <div style=margin-top:0;>tom@macwright.com</div>
            </div>
            <nav class=header-wrap>
                <div class="header nu limiter no-print">
                    <h2 style="line-height:1.6;font-size:1rem;margin:0 0 0.25em 0;">
                        <a href=/>Tom MacWright</a>
                    </h2>
                    <ul style=list-style:none;padding:0;margin:0;>
                        <li>
                            <a href=/writing>Writing</a>
                        </li>
                        <li>
                            <a href=/reading/>Reading</a>
                        </li>
                        <li>
                            <a href=/photos/>Photos</a>
                        </li>
                        <li>
                            <a href=/projects/>Projects</a>
                        </li>
                        <li>
                            <a href=/drawings/>Drawings</a>
                        </li>
                        <li>
                            <a href=/micro/>Micro</a>
                        </li>
                        <li>
                            <a href=/about/>About</a>
                        </li>
                    </ul>
                </div>
            </nav>
            <div class="pad2y limiter content">
                <a href=/writing/ class=front-page-title>Writing ⇢</a>
                <div class="writing nu">
                    <div>
                        <a href='/2025/06/06/recently' title='#10'>Recently</a>
                    </div>
                    <time>2025-06-06</time>
                    <div>
                        <a href='/2025/05/18/sewing' title='#9'>Making a custom porteur bag</a>
                    </div>
                    <time>2025-05-18</time>
                    <div>
                        <a href='/2025/05/02/reading-zanzibar' title='#8'>Reading Zanzibar</a>
                    </div>
                    <time>2025-05-02</time>
                    <div>
                        <a href='/2025/05/01/recently' title='#7'>Recently</a>
                    </div>
                    <time>2025-05-01</time>
                    <div>
                        <a href='/2025/04/12/tidbyt-second-life' title='#6'>Tidbyt without the company</a>
                    </div>
                    <time>2025-04-12</time>
                    <div>
                        <a href='/2025/04/07/recently' title='#5'>Recently</a>
                    </div>
                    <time>2025-04-07</time>
                    <div>
                        <a href='/2025/04/03/personal-tools' title='#4'>Personal tools</a>
                    </div>
                    <time>2025-04-03</time>
                    <div>
                        <a href='/2025/03/07/blogroll' title='#3'>Introducing the blogroll</a>
                    </div>
                    <time>2025-03-07</time>
                    <div>
                        <a href='/2025/03/01/recently' title='#2'>Recently</a>
                    </div>
                    <time>2025-03-01</time>
                    <div>
                        <a href='/2025/02/04/recently' title='#1'>Recently</a>
                    </div>
                    <time>2025-02-04</time>
                </div>
                <br>
                <a href=/micro/ class=front-page-title>Micro ⇢</a>
                <div class="writing nu">
                    <div>
                        <a href='/2025/06/26/zohran' title='#5'>The election</a>
                    </div>
                    <time>2025-06-26</time>
                    <div>
                        <a href='/2025/05/29/putting-an-untrusted-chat-layer-is-a-disaster' title='#4'>Putting an untrusted layer of chatbot AI between you and the internet is an obvious disaster waiting to happen</a>
                    </div>
                    <time>2025-05-29</time>
                    <div>
                        <a href='/2025/05/28/dont-rank-cuomo-vote-for-everyone-else' title='#3'>NYC Primaries June 24 - don't rank Cuomo, vote for everyone else</a>
                    </div>
                    <time>2025-05-28</time>
                    <div>
                        <a href='/2025/05/22/blog-micro-optimization' title='#2'>Blog micro-optimization</a>
                    </div>
                    <time>2025-05-22</time>
                    <div>
                        <a href='/2025/05/20/leader-key' title='#1'>LeaderKey.app is a very good launcher</a>
                    </div>
                    <time>2025-05-20</time>
                </div>
                <br>
                <a href=/photos/ class=front-page-title>Photos ⇢</a>
                <div class=front-page-images>
                    <div>
                        <a href='/2025/02/19/golconda'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-02-19-golconda_640.webp type=image/webp>
                                <img alt="Golconda Fort" loading=lazy src=https://images.macwright.com/2025-02-19-golconda_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2025/01/10/daulatabad'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-01-10-daulatabad_640.webp type=image/webp>
                                <img alt="Daulatabad Fort" loading=lazy src=https://images.macwright.com/2025-01-10-daulatabad_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2025/01/07/tomb'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-01-07-tomb_640.webp type=image/webp>
                                <img alt=Tomb loading=lazy src=https://images.macwright.com/2025-01-07-tomb_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2024/11/13/boat'>
                            <picture>
                                <source srcset=https://images.macwright.com/2024-11-13-boat_640.webp type=image/webp>
                                <img alt=Boat loading=lazy src=https://images.macwright.com/2024-11-13-boat_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2024/10/20/pier'>
                            <picture>
                                <source srcset=https://images.macwright.com/2024-10-20-pier_640.webp type=image/webp>
                                <img alt=Pier loading=lazy src=https://images.macwright.com/2024-10-20-pier_640.jpg>
                            </picture>
                        </a>
                    </div>
                </div>
                <br>
                <a href=/drawings/ class=front-page-title>Drawings ⇢</a>
                <div class=front-page-images>
                    <div>
                        <a href='/2025/04/16/bob-ross'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-04-16-bob-ross-x_640.webp type=image/webp>
                                <img alt="Bob Ross" loading=lazy src=https://images.macwright.com/2025-04-16-bob-ross-x_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2025/04/08/street'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-04-08-street_640.webp type=image/webp>
                                <img alt=Street loading=lazy src=https://images.macwright.com/2025-04-08-street_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2025/03/23/buttercups'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-03-23-buttercups_640.webp type=image/webp>
                                <img alt=Buttercups loading=lazy src=https://images.macwright.com/2025-03-23-buttercups_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2025/03/12/gibson'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-03-12-gibson_640.webp type=image/webp>
                                <img alt="Gibson girl" loading=lazy src=https://images.macwright.com/2025-03-12-gibson_640.jpg>
                            </picture>
                        </a>
                    </div>
                    <div>
                        <a href='/2025/03/10/fish'>
                            <picture>
                                <source srcset=https://images.macwright.com/2025-03-10-fish-two_640.webp type=image/webp>
                                <img alt=Fish loading=lazy src=https://images.macwright.com/2025-03-10-fish-two_640.jpg>
                            </picture>
                        </a>
                    </div>
                </div>
                <br>
                <a href=/reading/ class=front-page-title>Reading ⇢</a>
                <div class="books nu">
                    <div>
                        <a href='/2025/06/29/things-become-other-things'>Things Become Other Things</a>
                    </div>
                    <div>Craig Mod</div>
                    <time>2025-06-29</time>
                    <div>
                        <div class=star style=width:65px></div>
                    </div>
                    <div>
                        <a href='/2025/06/21/glass-century'>Glass Century</a>
                    </div>
                    <div>Ross Barkan</div>
                    <time>2025-06-21</time>
                    <div>
                        <div class=star style=width:65px></div>
                    </div>
                    <div>
                        <a href='/2025/05/16/abundance'>Abundance</a>
                    </div>
                    <div>Ezra Klein and Derek Thompson</div>
                    <time>2025-05-16</time>
                    <div>
                        <div class=star style=width:39px></div>
                    </div>
                    <div>
                        <a href='/2025/04/06/careless-people'>Careless People</a>
                    </div>
                    <div>Sarah Wynn-Williams</div>
                    <time>2025-04-06</time>
                    <div>
                        <div class=star style=width:52px></div>
                    </div>
                    <div>
                        <a href='/2025/03/22/land-is-a-big-deal'>Land is a Big Deal</a>
                    </div>
                    <div>Lars A. Doucet</div>
                    <time>2025-03-22</time>
                    <div>
                        <div class=star style=width:52px></div>
                    </div>
                </div>
            </div>
        </div>
    </body>
</html>
