<template>
 
    
 <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img class="d-block w-100" src="../../../assets/img/banner/banner.png" alt="Premier diaporama">
                <!-- Contenu centré -->
                <div class="carousel-caption d-flex flex-column justify-content-center align-items-center">
                    <h3>Indonesia</h3>
                    <p>The natural wonders of the archipelago</p>
                    <a href="#" class="btn btn-primary" id="btn">Explorer maintenant</a>
                </div>
            </div>
            <div class="carousel-item">
                <img class="d-block w-100" src="../../../assets/img/banner/banner2.png" alt="Deuxième diaporama">
                <!-- Contenu centré -->
                <div class="carousel-caption d-flex flex-column justify-content-center align-items-center">
                    <h3>Désert</h3>
                    <p>Journey Through the Desert</p>
                    <a href="#" class="btn btn-primary" id="btn">Explorer maintenant</a>
                </div>
            </div>
            <div class="carousel-item">
                <img class="d-block w-100" src="../../../assets/img/banner/banner4.png" alt="Troisième diaporama">
                <!-- Contenu centré -->
                <div class="carousel-caption d-flex flex-column justify-content-center align-items-center">
                    <h3>Cappadocia</h3>
                    <p>exploring Cappadocia's Unique Beauty</p>
                    <a href="#" class="btn btn-primary" id="btn">Explorer maintenant</a>
                </div>
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Précédent</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Suivant</span>
        </a>
    </div>




    
     <!-- popular_destination_area_start  -->
    <div class="popular_destination_area">
        <div class="container">
    <div class="row justify-content-center">
        <div class="col-lg-6">
            <div class="section_title text-center mb_70">
                <h3>Let’s Travel Together</h3>
                <p>Let’s travel together and explore new destinations, uncover hidden gems, and create unforgettable memories.</p>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-4 col-md-6">
            <router-link to="/Destination" >
            <div class="single_destination">
                
                <div class="thumb">
                    <img src="../../../img/destination/1.png" alt="">
                </div>
                <div class="content">
                    <p class="d-flex align-items-center">Italie  </p>
                </div>
            
            </div>
        </router-link>
        </div>
        <div class="col-lg-4 col-md-6">
            <router-link to="/Destination" >
            <div class="single_destination">
                <div class="thumb">
                    <img src="../../../img/destination/2.png" alt="">
                </div>
                <div class="content">
                    <p class="d-flex align-items-center">Brésil</p>
                </div>
            </div>
        </router-link>
        </div>
        <div class="col-lg-4 col-md-6">
            <router-link to="/Destination" >
            <div class="single_destination">
                <div class="thumb">
                    <img src="../../../img/destination/3.png" alt="">
                </div>
                <div class="content">
                    <p class="d-flex align-items-center">Australia </p>
                </div>
            </div>
        </router-link>
        </div>
        <div class="col-lg-4 col-md-6">
            <router-link to="/Destination" >
            <div class="single_destination">
                <div class="thumb">
                    <img src="../../../img/destination/4.png" alt="">
                </div>
                <div class="content">
                    <p class="d-flex align-items-center">Népal </p>
                </div>
            </div>
        </router-link>
        </div>
        <div class="col-lg-4 col-md-6">
            <router-link to="/Destination" >
            <div class="single_destination">
                <div class="thumb">
                    <img src="../../../img/destination/5.png" alt="">
                </div>
                <div class="content">
                    <p class="d-flex align-items-center">Marocoo</p>
                </div>
            </div>
        </router-link>
        </div>
        <div class="col-lg-4 col-md-6">
            <router-link to="/Destination" >
            <div class="single_destination">
                <div class="thumb">
                    <img src="../../../img/destination/6.png" alt="">
                </div>
                <div class="content">
                    <p class="d-flex align-items-center">Indonésie </p>
                </div>
            </div>
        </router-link>
        </div>
    </div>
</div>

    </div>
    <!-- popular_destination_area_end  -->

    <!-- newletter_area_start  -->
    <div class="newletter_area overlay">
        <div class="container">
            <div class="row justify-content-center align-items-center">
                <div class="col-lg-10">
                    <div class="row align-items-center">
                       
                        <div class="col-lg-7">
                            <div class="mail_form">
                                <div class="row no-gutters">
                                   
                                    <div class="col-lg-3 col-md-4">
                                        <div class="newsletter_btn">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- newletter_area_end  -->

    <div class="popular_places_area">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-6">
                    <div class="section_title text-center mb_70">
                        <h3>Lieux populaires</h3>
                        <p>Modification subie sous une certaine forme, par humour injecté ou bons mots de barbe de lune de loup de 8 bits d'animation de stand aléatoire de bonne journée.</p>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-lg-4 col-md-6" v-for="vole in voles.slice(0, 6)" :key="vole.id">
                    <div class="single_place">
                        <div class="thumb">
                            <img :src="`http://localhost:8000/images/${vole.image}`" alt="" v-if="vole.image" />
                            <a href="#" class="prise">{{ vole.prix }}$</a>
                        </div>
                        <div class="place_info">
                            <a :href="`/Gallry/${vole.id}`"><h3>{{ vole.ville }}</h3></a>
                            <p>{{ vole.description }}</p>
                        <div class="rating_days d-flex justify-content-between">
                             <span class="d-flex justify-content-center align-items-center">
                                <i class="fa fa-star" v-for="n in 5" :key="n"></i>
                                <a href="#">(20 Review)</a>
                            </span>
                            <div class="days">
                                <i class="fa fa-clock-o"></i>
                                <a href="#">{{ vole.duree }} Days</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            </div>
            <div class="row">
                <div class="col-lg-12">
                    <div class="more_place_btn text-center">
                        <a class="boxed-btn4" href="#">More Places</a>
                    </div>
                </div>
            </div>
        </div>
    </div>


    <div class="video_area video_bg overlay">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="video_wrap text-center">
                        <h3>Enjoy view</h3>
                       
                    </div>
                </div>
            </div>
        </div>
    </div>


    <div class="travel_variation_area">
        <div class="container">
            <div class="row">
                <div class="col-lg-4 col-md-6">
                    <div class="single_travel text-center">
                        <div class="icon">
                            <img src="../../../img/svg_icon/1.svg" alt="">
                        </div>
                        <h3>Comfortable Journey</h3>
                        <p>A wonderful serenity has taken to the possession of my entire soul.</p>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6">
                    <div class="single_travel text-center">
                        <div class="icon">
                            <img src="../../../img/svg_icon/2.svg" alt="">
                        </div>
                        <h3>Luxuries Hotel</h3>
                        <p>A wonderful serenity has taken to the possession of my entire soul.</p>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6">
                    <div class="single_travel text-center">
                        <div class="icon">
                            <img src="../../../img/svg_icon/3.svg" alt="">
                        </div>
                        <h3>Travel Guide</h3>
                        <p>A wonderful serenity has taken to the possession of my entire soul.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>


    




</template>

<script>
import axios from 'axios';
export default{
    data() {
       return {
          voles: [],
        }
    },
    mounted() {
        this.fetchVoles(); // Fetch the voles when the component is mounted
    },
    methods:{
        fetchVoles() {
            axios.get('http://localhost:8000/api/voles') // Adjust the URL as needed
                .then(response => {
                this.voles = response.data; // Store the fetched voles
            })
                .catch(error => {
                console.error('Error fetching voles:', error);
            });
        }
    }
}
</script>
<style>  
.carousel-item img {
    height: 500px; /* Adjust the height as needed */
    object-fit: cover; /* Ensure the image covers the container without distortion */
  }
    .carousel-caption {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
    }

    .carousel-caption h3 {
        font-size: 3rem;
        color: #fff;
    }

    .carousel-caption p {
        color: #fff;
        margin-bottom: 20px;
    }

    .carousel-caption a.btn {
        padding: 10px 20px;
    }
</style>