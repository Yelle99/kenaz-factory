<template>
  <article class="singlenews">
    <div class="text-content">
      <p class="single-text">
        Vestibulum id ligula porta felis euismod semper. Morbi leo risus, porta
        ac consectetur ac, vestibulum at eros. Aenean lacinia bibendum nulla sed
        consectetur.Sed posuere consectetur est at lobortis. Donec sed odio dui.
        Aenean lacinia bibendum nulla sed consectetur. Cras justo odio, dapibus
        ac facilisis in, egestas eget quam. Donec sed odio dui. Vivamus sagittis
        lacus vel augue laoreet rutrum faucibus dolor auctor. Cras justo odio,
        dapibus ac facilisis in, egestas eget quam. Donec sed odio dui. Nulla
        vitae elit libero, a pharetra augue. Curabitur blandit tempus porttitor.
        Nulla vitae elit libero, a pharetra augue. Nullam quis risus eget urna
        mollis ornare vel eu leo.
      </p>
      <img src="../assets/notebook.png" alt="" />
      <p class="single-text">
        Molestias ultricies, ante quam urna ut volutpat, egestas dolor dui, nec
        hac ultrices nulla non netus. Placerat vehicula donec non suscipit
        egestas, augue vel suspendisse. Et felis venenatis blandit sed est
        ultrices, adipiscing urna, at aliquam nullam facilisis aliquet sapien,
        eget duis consectetuer tristique nunc vitae erat, mi purus nisl lorem.
        Ac magna lobortis non, vulputate vitae viverra. Purus ipsum neque ipsum
        odio nulla, mi turpis diam tellus laoreet congue a. Rhoncus maecenas,
        sit suspendisse, condimentum purus convallis dui hendrerit. Purus ipsum
        neque ipsum odio nulla, mi turpis diam tellus laoreet congue.
      </p>
    </div>
    <div class="banner-news"></div>
    <div class="author">
      <h1>About the Author</h1>
      <div class="author-info">
        <img src="../assets/author.png" alt="" />
        <p>
          Molestias ultricies, ante quam urna ut volutpat, egestas dolor dui,
          nec hac ultrices nulla non netus. Placerat vehicula donec non suscipit
          egestas, augue vel suspendisse. Et felis venenatis blandit sed est
          ultrices, adipiscing urna, at aliquam nullam facilisis aliquet sapien,
          eget duis consectetuer tristique nunc vitae erat, mi purus nisl lorem.
        </p>
      </div>
    </div>
    <div class="comments">
      <h1>Comments</h1>
      <div class="comment">
        <div class="image-container">
          <div class="image">
            <img src="../assets/person.png" alt="" />
          </div>
        </div>
        <div class="text-container">
          <div class="comment-author">
            <p class="name">Matt Adams</p>
            <p class="comment-date">Jan 2nd, 2012 2:35 pm</p>
            <button class="reply">Reply</button>
          </div>
          <p class="comment-text">
            Molestias ultricies, ante quam urna ut volutpat, egestas dolor dui,
            nec hac ultrices nulla non netus. Placerat vehicula donec non
            suscipit egestas, augue vel suspendisse. Et felis venenatis blandit
            sed est ultrices, adipiscing urna.
          </p>
        </div>
      </div>
      <div class="comment">
        <div class="image-container">
          <div class="image">
            <img src="../assets/person.png" alt="" />
          </div>
        </div>
        <div class="text-container">
          <div class="comment-author">
            <p class="name">John Toews</p>
            <p class="comment-date">Jan 2nd, 2012 2:35 pm</p>
            <button class="reply">Reply</button>
          </div>
          <p class="comment-text">
            Molestias ultricies, ante quam urna ut volutpat, egestas dolor dui,
            nec hac ultrices nulla non netus. Placerat vehicula donec non
            suscipit egestas, augue vel suspendisse. Et felis venenatis blandit
            sed est ultrices, adipiscing urna.
          </p>
        </div>
      </div>
      <div class="comment">
        <div class="image-container">
          <div class="image">
            <img src="../assets/person.png" alt="" />
          </div>
        </div>
        <div class="text-container">
          <div class="comment-author">
            <p class="name">Andrew Enns</p>
            <p class="comment-date">Jan 2nd, 2012 2:35 pm</p>
            <button class="reply">Reply</button>
          </div>
          <p class="comment-text">
            Molestias ultricies, ante quam urna ut volutpat, egestas dolor dui,
            nec hac ultrices nulla non netus. Placerat vehicula donec non
            suscipit egestas, augue vel suspendisse. Et felis venenatis blandit
            sed est ultrices, adipiscing urna.
          </p>
        </div>
      </div>
      <div class="add-comment">
        <h1>Add Your Comment</h1>
        <p>
          Molestias ultricies, ante quam urna ut volutpat, egestas dolor dui,
          nec hac ultrices nulla non netus. Placerat vehicula donec non suscipit
          egestas, augue vel suspendisse. Et felis venenatis blandit sed est
          ultrices, adipiscing urna.
        </p>
        <form>
          <input placeholder="Name" type="text" />
          <input placeholder="Email Address" type="text" />
          <input class="comment-input" placeholder="Comment" type="text" />
          <button type="submit">Submit</button>
        </form>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  name: "SingleNews",
};
</script>
