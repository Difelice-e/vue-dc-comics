<template>
    <footer class="footer">
        <div class="footer__link">
            <div class="container">
                <ul class="nav__menu">
                    <li v-for="(item, i) in footerMenu" :key="i">
                        <h4>{{item.title}}</h4>
                        <ul class="nav__link">
                            <li v-for="(link, i) in item.links" :key="i">
                                <a :href="link.href">{{ link.name }}</a>
                            </li>
                        </ul>      
                    </li>
                </ul>
            </div>
        </div>

        <div class="footer__social">
            <div class="container">
                <button>
                    <a href="#">
                        Sign-up now!
                    </a>
                </button>

                <ul class="social__link">
                    <li>
                        <a href="#">FOLLOW US</a>
                    </li>  
                    <li v-for="(item, i) in socialMenu" :key="i">
                        <a :href="item.href">
                            <img :src="require(`../assets/img/${item.icon}`)" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'PageFooter',
    data() {
        return {
            footerMenu: [
                {
                    title: 'DC Comics',
                    links: [
                        {
                            name: 'Characters',
                            href: '#'
                        },
                        {
                            name: 'Comics',
                            href: '#'
                        },
                        {
                            name: 'Movies',
                            href: '#'
                        },
                        {
                            name: 'TV',
                            href: '#'
                        },
                        {
                            name: 'Games',
                            href: '#'
                        },
                        {
                            name: 'Videos',
                            href: '#'
                        },
                        {
                            name: 'News',
                            href: '#'
                        },
                    ]
                },
                {
                    title: 'Shop',
                    links: [
                        {
                            name: 'Shop DC',
                            href: '#'
                        },
                        {
                            name: 'Shop DC Collectibles',
                            href: '#'
                        },
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        {
                            name: 'CTerms Of Use',
                            href: '#'
                        },
                        {
                            name: 'Privacy Policy (new)',
                            href: '#'
                        },
                        {
                            name: 'Ad Choices',
                            href: '#'
                        },
                        {
                            name: 'Advertising',
                            href: '#'
                        },
                        {
                            name: 'Jobs',
                            href: '#'
                        },
                        {
                            name: 'Subscriptions',
                            href: '#'
                        },
                        {
                            name: 'Talent Workshops',
                            href: '#'
                        },
                        {
                            name: 'CPSC Certificates',
                            href: '#'
                        },
                        {
                            name: 'Ratings',
                            href: '#'
                        },
                        {
                            name: 'Shop Help',
                            href: '#'
                        },
                        {
                            name: 'Contact Us',
                            href: '#'
                        },
                    ]
                },
                {
                    title: 'Sites',
                    links: [
                        {
                            name: 'DC',
                            href: '#'
                        },
                        {
                            name: 'MAD Magazine',
                            href: '#'
                        },
                        {
                            name: 'DC Kids',
                            href: '#'
                        },
                        {
                            name: 'DC Universe',
                            href: '#'
                        },
                        {
                            name: 'DC Power Visa',
                            href: '#'
                        },
                    ]
                },
            ],
            socialMenu: [
                {
                    name: 'facebook',
                    href: '#',
                    icon: 'footer-facebook.png'
                },
                {
                    name: 'twitter',
                    href: '#',
                    icon: 'footer-twitter.png'
                },
                {
                    name: 'youtube',
                    href: '#',
                    icon: 'footer-youtube.png'
                },
                {
                    name: 'pinterest',
                    href: '#',
                    icon: 'footer-pinterest.png'
                },
                {
                    name: 'periscope',
                    href: '#',
                    icon: 'footer-periscope.png'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.footer {

    .footer__link {
        background-image: url('../assets/img/footer-bg.jpg');
        padding: 30px 10px 50px;

        .nav__menu {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            height: 280px;
            width: 380px;
            gap: 10px;
            list-style: none;
            
            h4 {
                text-transform: uppercase;
                color: white;
                margin-bottom: 15px;
            }

            .nav__link {
                margin-bottom: 15px;
                list-style: none;

                a {
                    color: #626F7C;
                    text-decoration: none;
                    font-size: 0.7rem;
                }
            }
        }

    }

    .footer__social {
        background-color: var(--app-heavy-grey);
        padding: 30px 10px;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        
            button {
            text-transform: uppercase;
            background-color: transparent;
            border: 2px solid;
            border-color: var(--app-blue);
            padding: 8px;
            
                a {
                    text-decoration: none;
                    color: white;
                    font-weight: 600;
                
                }
            }

            .social__link {
                display: flex;
                align-items: center;
                gap: 18px;
                list-style: none;

                a {
                    text-decoration: none;
                    color: var(--app-blue);
                    font-weight: 600;
                }
            }
        }

        
    }
}
</style>