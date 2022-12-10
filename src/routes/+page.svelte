<script>
    import programmer from '$lib/assets/programmer.svg'
</script>

<svelte:head>
    <title>FeriVOQ</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
</svelte:head>

<main>
    <div class="outer">
        <div class="middle">
          <div class="inner">
            <strong class="hi">Hi there👋, I am</strong>
            <h1 class="name">ferivoq.</h1>
            <strong class="job">Front-end web developer 🧑‍💻</strong>
            <p class="desc">I am a Front-end web developer and a Newbie Designer <br> based in Hungary, Budapest.</p>
        </div>
      </div>
      <div class="img">
        <img
            src={programmer} 
            alt="ProgrammerPic"
         >
      </div>
    
    <div>
        <p class="footer">Made with Svelte ❤️</p>
    </div>
</main>

<style global>
    :global(body) {
        background-color: black;
    }
    .hi {
        color: white;
        text-transform: uppercase;
        font-family: 'Roboto', sans-serif;
        font-weight: normal;
        letter-spacing: 3px;
        font-size: 12px;
    }
    .name {
        color: white;
        font-family: 'Roboto', sans-serif;
        font-weight: 900;
        font-size: 70px;
        margin-top: 30px;
        margin-bottom: 30px;
    }
    .job {
        color: #77ED6A;
        text-transform: uppercase;
        font-family: 'Roboto', sans-serif;
        font-weight: bold;
        letter-spacing: 5px;
        font-size: 14px;
        
    }
    .desc {
        color: #787878;
        font-family: 'Roboto', sans-serif;
        font-weight: normal;
        font-size: 14px;
        margin-top: 25px;
    }
    .outer {
        display: table;
        position: absolute;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
    }

    .middle {
        display: table-cell;
        vertical-align: middle;
    }

    .inner {
        margin-left: 140px;
    }
    .img {
        position: absolute;
        top: 50%;
        transform: translate(-115%, -50%);
    }

    .footer {
        position: fixed;
        left: 0;
        bottom: 0;
        width: 100%;
        color: #787878;
        font-family: 'Roboto', sans-serif;
        font-size: 15px;
        text-align: center;
    }

    @media (max-width: 1180px) {
    .img {
        display: none;
    }
    .inner {
        text-align: center;
        margin-left: 0;
    }
}

    @media (max-width: 285px) {
    .hi {
        font-size: 8px;
    }
    .name {
        font-size: 66px;
    }
    .job {
        font-size: 10px;
    }
    .desc {
        font-size: 9px;
    }
}

    @media only screen and (max-height: 305px) {
    .name {
        margin-top: 5px;
        margin-bottom: 5px;
    }
    .desc {
        margin-top: 15px;
    }
}

    @media only screen and (max-height: 587px) {
    .img {
        display: none;
    }   
}
</style>