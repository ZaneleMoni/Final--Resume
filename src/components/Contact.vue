<template>
  <!-- ======= Contact Section ======= -->
  <section id="contact" class="contact">
    <div class="container">
      <div class="section-title">
        <h2>Contact</h2>
        <!-- <p>Magnam dolores commodi suscipit. Necessitatibus eius consequatur ex aliquid fuga eum quidem. Sit sint consectetur velit. Quisquam quos quisquam cupiditate. Et nemo qui impedit suscipit alias ea. Quia fugiat sit in iste officiis commodi quidem hic quas.</p> -->
      </div>

      <form >
        <div class="row mt-5">
          <div class="col-lg-4">
            <div class="info">
              <div class="address">
                <i class="bi bi-geo-alt"></i>
                <h4>Location:</h4>
                <p>Cape Town</p>
              </div>

              <div class="email">
                <i class="bi bi-envelope"></i>
                <h4>Email:</h4>
                <p>zanelemoni4@gmail.com</p>
              </div>

              <div class="phone">
                <i class="bi bi-phone"></i>
                <h4>Call:</h4>
                <p>+27 62 433 4358</p>
              </div>
            </div>
          </div>

          <div class="col-lg-7 mt-5 mt-lg-0">
            <form @submit.prevent="handleSubmit"
              action="forms/contact.php"
              method="post"
              role="form"
              class="php-email-form"
            >
              <div class="row">
                <div class="col-md-6 form-group">
                  <input
                    type="text"
                    name="name"
                    class="form-control"
                    v-model="name"
                    id="name"
                    placeholder="Your Name"
                    required
                  />
                </div>
                <div class="col-md-6 form-group mt-3 mt-md-0">
                  <input
                    type="email"
                    class="form-control"
                    name="email"
                    v-model="email"
                    id="email"
                    placeholder="Your Email"
                    required
                  />
                </div>
              </div>
             
              <div class="form-group mt-3">
                <textarea
                  class="form-control"
                  name="message"
                  rows="5"
                  v-model="message"
                  placeholder="Message"
                  required
                ></textarea>
              </div>
              <div class="my-3">
                <div class="loading">Loading</div>
                <div class="error-message"></div>
                <div class="sent-message">
                  Your message has been sent. Thank you!
                </div>
              </div>
              <div class="text-center">
                <button type="submit">Send Message</button>
              </div>
            </form>
          </div>
        </div>
      </form>
    </div>
  </section>
  <!-- End Contact Section -->
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
  methods: {
    handleSubmit() {
      console.log(this.name, this.email, this.message);
      this.name = "";
      this.email = "";
      this.message = "";

      fetch("http://localhost:8000/contact", {
        method: "POST",
        body: JSON.stringify({
          name: this.name,
          email: this.email,
          message: this.message,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((response) => response.json())
        .then((json) => console.log(json))
        .catch((e) => alert(e.msg));
    },
  },
};
</script>

<style>
#contact{
  padding: 71px;
}
.contact .info {
  width: 100%;
  background: #fff;
}
.contact .info i {
  font-size: 20px;
  color: #34b7a7;
  float: left;
  width: 44px;
  height: 44px;
  background: #effbf9;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
  transition: all 0.3s ease-in-out;
}
.contact .info h4 {
  padding: 0 0 0 60px;
  font-size: 22px;
  font-weight: 600;
  margin-bottom: 5px;
  color: #222222;
}
.contact .info p {
  padding: 0 0 0 60px;
  margin-bottom: 0;
  font-size: 14px;
  color: #555555;
}
.contact .info .email,
.contact .info .phone {
  margin-top: 40px;
}
.contact .info .email:hover i,
.contact .info .address:hover i,
.contact .info .phone:hover i {
  background: #34b7a7;
  color: #fff;
}
.contact .php-email-form {
  width: 100%;
  background: #fff;
}
.contact .php-email-form .form-group {
  padding-bottom: 8px;
}
.contact .php-email-form .error-message {
  display: none;
  color: #fff;
  background: #ed3c0d;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}
.contact .php-email-form .sent-message {
  display: none;
  color: #fff;
  background: #18d26e;
  text-align: center;
  padding: 15px;
  font-weight: 600;
}
.contact .php-email-form .loading {
  display: none;
  background: #fff;
  text-align: center;
  padding: 15px;
}
.contact .php-email-form .loading:before {
  content: "";
  display: inline-block;
  border-radius: 50%;
  width: 24px;
  height: 24px;
  margin: 0 10px -6px 0;
  border: 3px solid #18d26e;
  border-top-color: #eee;
  -webkit-animation: animate-loading 1s linear infinite;
  animation: animate-loading 1s linear infinite;
}
.contact .php-email-form input,
.contact .php-email-form textarea {
  border-radius: 4px;
  box-shadow: none;
  font-size: 14px;
}
.contact .php-email-form input:focus,
.contact .php-email-form textarea:focus {
  border-color: #34b7a7;
}
.contact .php-email-form input {
  height: 44px;
}
.contact .php-email-form textarea {
  padding: 10px 12px;
}
.contact .php-email-form button[type="submit"] {
  background: #34b7a7;
  border: 0;
  padding: 10px 30px 12px 30px;
  color: #fff;
  transition: 0.4s;
  border-radius: 50px;
}
.contact .php-email-form button[type="submit"]:hover {
  background: #3dc8b7;
}
@-webkit-keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
@keyframes animate-loading {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
</style>
