<template>
    <div class="container-fluid">
    <div class="row">
        <div class="col-md-12 d-flex justify-content-center right-bck">
            <div class="registration-right">
               
                <div class="event-list">
                    <div class="card flex-row"><img class="card-img-left img-fluid" :src="post.urlToImage" />
                        <div class="card-body card-padding-right-left-remover">
                          

                            <div class="container card-padding-right-left-remover">
                                <div class="row">
                                  <div class="col-2">
                                    <!-- {{ post.author }} -->
                                  </div>
                                    <div class="col-8">
                                   <strong> {{ post.title }} </strong>  
                                  </div>
                                  <div class="col-2 card-padding-right-left-remover">
                                  <h4 class="card-title h5 h4-sm pushright"><i class="fas fa-caret-right" aria-hidden="true"></i><span>{{post.publishedAt.substring(0,10)}}</span></h4>
                                  </div>
                                </div>
                              </div>
                              <br>
                              <div class="container">
                                {{ post.description }}

                              </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<script>
export default {

  props: ["post"],

}
</script>

<style scoped>
.card-padding-right-left-remover{
padding-right: 0 !important;
padding-left: 0 !important
}

.pushright{
  right: 1% !important
}
.right-bck {
    background-color: #F1f9ec
}

.registration-right {
    width: 80%;
    margin-bottom: 1.5%;
    margin-top: 1.5;
}

.registration-right h2 {
    color: #ffffff;
    font-weight: 700;
    padding-bottom: 20px
}

.registration .btn {
    width: 100%
}

.fa,
.fas,
.fab {
    font-family: "Font Awesome 5 Free";
    font-weight: 900
}

.far {
    font-family: "Font Awesome 5 Free";
    font-weight: 400
}

.event-list .card {
    background-color: #ffffff;
    padding: 18px;
    margin-bottom: 3px;
    box-shadow: 5px 5px 15px 5px rgba(0,0,0,0.43);
}

.event-list img {
    width: 77px;
    height: 77px
}

.event-list h4 {
    color: #020202;
    font-size: 16px
}

.event-list .card-title span {
    padding-left: 5px;
    padding-right: 20px;
    font-size: 12px;
    font-weight: 700
}

.event-list .card-text {
    color: #000000;
    font-weight: 700;
    font-size: 16px
}

.event-list .card-body {
    padding: 0 20px;
    margin: 0 0 10px 0

}

.event-list .card-title svg {
    color: #ffffff
}
</style>