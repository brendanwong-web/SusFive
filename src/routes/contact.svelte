<svelte:head>
	<title>Contact Us</title>
</svelte:head>

<script>
    	import Button from '../components/Button.svelte';
</script>

<style lang="scss" global>
    @import "./style/theme.scss";
        
    .container.contact {
        padding: 6rem 0 0;
        width: 100vw;
        position: relative;
        overflow-y: scroll;
        @media screen and (min-width: 560px) {
            padding: 5rem 10vw 0 10vw;
            width: 100vw;
            height: 100vh;
            position: relative;
            overflow-y: scroll;
            overflow-x: hidden;
        }
    }

    .card-con {
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        margin-top: 0rem;
        min-height: 55vh;

        @media screen and (min-width: 560px) {
            width: 100%;
            display: flex;
            flex-direction: row;
            justify-content: space-around;
            align-items: stretch;
            margin-top: 0rem;
            min-height: 55vh;
        }
        
    }

    .card-wrapper {
        padding: 15px;
        max-width: 99vw;
        flex: 1 1 100%;
        
        @media screen and (min-width: 560px) {
            padding: 0 0.5rem;
            max-width: 250px;
            flex: 1 1 100%;
        }
    }

    form {
        margin: 0;
        width: 100vw;
        padding: 2rem;
        background-color: $green-2;
        height: 450px;


        @media screen and (min-width: 560px) {
            margin: -6rem -10vw 0 -10vw;
            bottom: 0;
            left: 0;
            content: '';
            width: 100vw;
            padding: 10em 10vw;
            background-color: $green-2;
            height: 600px;
        }

        .formgrp {
            display: flex;
            flex-direction: column;
            max-width: 500px;
            margin-bottom: 20px;

            label {
            font-size:1rem;
            text-transform: uppercase;
            font-weight: 700;
            margin-bottom: 5px;
            }

            input,
            textarea {
                padding: 0.5rem;
                color: rgb(64, 64, 64);
                outline: none;
                border: none;
                border-radius: 15px;
                box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
            }
        }

        
    }

    .card {
        min-height: 300px;
        height: 100%;
        border: 1px solid $green-3;
        border-radius: 7px;
        padding: 20px;
        background-color: white;

        .top {
            clip-path: circle(130px at 50% 50%);
            width: 100%;
            min-height: 300px;
            @media screen and (min-width: 560px) {
                clip-path: circle(80px at 50% 50%);
                width: 100%;
                min-height: 170px;
            }

            img {
                width: 100%;
                height: auto;
            }
        }

        .name {
            p {
                font-weight: 600;
                font-size: 1.5rem;
                margin-bottom: 0;

                @media screen and (min-width: 560px) {
                    font-size: 1rem;
                }

                span {
                    font-weight: 300;
                    font-size: 1rem;
                    font-style: italic;

                    @media screen and (min-width: 560px) {
                        font-size: 0.8rem;
                    }
                }
            }

            text-align: left;
        }

        .info {
            padding-top: 20px;
        }
    }


</style>


<div class="container contact">
    <div class="card-con">
        <div class="card-wrapper">

            <div class="card">
                <div class="top">
                    <img src="andrea.jpg" alt="profile">
                </div>
                <div class="bottom">
                  <div class="name">
                <p>Andrea Tan, <span>CEO</span></p>
                </div>
                <div class="info">
                    In charge of the company’s major decisions and corporate strategies
                </div>  
                </div>
                
            </div>
        </div>
        <div class="card-wrapper">

            <div class="card">
                <div class="top">
                    <img src="huifen.jpg" alt="profile">
                </div>
                <div class="bottom">
                  <div class="name">
                <p>Koh Hui Fen, <span>CFO</span></p>
                </div>
                <div class="info">
                    Responsible for the corporate treasury 
                </div>  
                </div>
                
            </div>
        </div>
        <div class="card-wrapper">

            <div class="card">
                <div class="top">
                    <img src="yingxuan.jpg" alt="profile">
                </div>
                <div class="bottom">
                  <div class="name">
                <p>Lim Ying Xuan, <span>COO</span></p>
                </div>
                <div class="info">
                    Responsible for the running of the day to day activities of the business
                </div>  
                </div>
                
            </div>
        </div>
        <div class="card-wrapper">

            <div class="card">
                <div class="top">
                    <img src="elsie.jpg" alt="profile">
                </div>
                <div class="bottom">
                  <div class="name">
                <p>Elsie Goh, <span>CMO </span></p>
                </div>
                <div class="info">
                    Responsible for corporate publicity and marketing 
                </div>  
                </div>
                
            </div>
        </div>
        <div class="card-wrapper">

            <div class="card">
                <div class="top">
                    <img src="sourav.jpg" alt="profile">
                </div>
                <div class="bottom">
                  <div class="name">
                <p>Sourav, <span>CLO </span></p>
                </div>
                <div class="info">
                    Executive Director responsible for ensuring corporate activities are in line with local laws.
                </div>  
                </div>
                
            </div>
        </div>
        

    </div>
    <form action="">
        <div class="formgrp">
            <label for="userEmail">Your Email</label>
            <input type="text" name='userEmail' placeholder="Leave blank if you wish to remain anonymous">
        </div>
        <div class="formgrp">
            <label for="text">Message</label>
            <textarea name="text" id="" cols="30" rows="10"></textarea>

        </div>
        <Button>Submit</Button>
    </form>
</div>