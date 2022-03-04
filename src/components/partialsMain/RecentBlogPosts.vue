<template>

    <div class="blog-post">

        <div class="containerPartials">

            <h4>tales from the barber shop</h4>
            <h2>recent blog posts</h2>

            <div class="display-containers">

                <div class="containerPartials services-items">

                    <img src="../../assets/img/avadabarbers-second-blog-700x441.jpg" alt="publicity">

                    <h3>avada barbers now open</h3>

                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

                </div>

                <div class="containerPartials services-items">

                    <img src="../../assets/img/avadabarbers-choosing-blog-700x441.jpg" alt="publicity">

                    <h3>chosing the right barber</h3>

                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

                </div>

                <div class="containerPartials services-items">

                    <img src="../../assets/img/avadabarbers-ourservice-blog-700x441.jpg" alt="publicity">

                    <h3>quick service guide</h3>

                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aspernatur impedit optio vitae tempore, itaque dolorum. Ullam sunt blanditiis animi harum autem repellat qui eligendi, adipisci incidunt eos quibusdam? Aliquam, nemo.</p>

                </div>

            </div>

            <button>read more from our blog</button>

        </div>

    </div>
    
</template>

<script>
export default {
    name: "RecentBlogPosts"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/variables.scss";

.blog-post {
    background-color: #f5f5f5;

    h2 {
        margin: -15px 0 20px;
    }

    .services-items {
    padding: 10px;
    width: $width3;
    max-width: 300px;

    img {
        height: auto;
        width: 100%;
    }

    h3 {
        width: 90%;
        font-size: 1.4rem;
        text-align: center;
    }
    }

    button {
        margin-top: 50px;
    }
}

</style>