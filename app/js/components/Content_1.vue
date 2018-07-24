<template>
    <div>
        <div class="container">

            <h1 class="my-4">Lorem ipsum dolor sit amet</h1>

            <div class="row d-none">
                <div class="col-lg-4 mb-4">
                    <div class="card h-100">
                        <h4 class="card-header">Card Title</h4>
                        <div class="card-body">
                            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</p>
                        </div>
                        <div class="card-footer">
                            <a href="#" class="btn btn-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 mb-4">
                    <div class="card h-100">
                        <h4 class="card-header">Card Title</h4>
                        <div class="card-body">
                            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis ipsam eos, nam perspiciatis
                                natus commodi similique totam consectetur praesentium molestiae atque exercitationem ut consequuntur,
                                sed eveniet, magni nostrum sint fuga.</p>
                        </div>
                        <div class="card-footer">
                            <a href="#" class="btn btn-primary">Learn More</a>
                        </div>
                    </div>
                </div>
                <div class="col-lg-4 mb-4">
                    <div class="card h-100">
                        <h4 class="card-header">Card Title</h4>
                        <div class="card-body">
                            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente esse necessitatibus neque.</p>
                        </div>
                        <div class="card-footer">
                            <a href="#" class="btn btn-primary">Learn More</a>
                        </div>
                    </div>
                </div>
            </div>

            <div class="row py-4">


                <div class="card" style="width: 18rem;" v-for="car in cars" v-bind:key="car.id">
                <img class="card-img-top" v-bind:src="car.image" alt="Card image cap">
                <div class="card-body">
                    <h5 class="card-title">{{ car.name }}</h5>
                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                </div>
                <ul class="list-group list-group-flush">
                    <li class="list-group-item">Cras justo odio</li>
                    <li class="list-group-item">Dapibus ac facilisis in</li>
                    <li class="list-group-item">Vestibulum at eros</li>
                </ul>
                <div class="card-body">
                    <a href="#" class="card-link">Card link</a>
                    <a href="#" class="card-link">Another link</a>
                </div>
                </div>




            </div>

        </div>

    </div>
</template>
<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      cars: [
        {
          id: 1,
          name: "Renault Megane",
          doors: 4,
          passangers: 5,
          image:
            "https://www.carbuyersguide.net/uploaded/nc_images/generations/large/renault-megane-10.png"
        },
        {
          id: 2,
          name: "Ford Focus",
          doors: 4,
          passangers: 6,
          image:
            "https://hips.hearstapps.com/amv-prod-cad-assets.s3.amazonaws.com/images/media/672264/2018-ford-focus-in-depth-model-review-car-and-driver-photo-693214-s-original.jpg"
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
