
<div class ="grid">
<!--iterate over this 6 times-->
    <div class="card">
        <div class="image"></div>
        <div class="info">
            <h1 class="name">Evil Rick</h1>
            <h3 class="status"><div class="dead"></div> Dead - Humanoid</h3>

            <h3 class="locationLabel">Last known location</h3>
            <h3 class="location"><li href="#">Citadel of Ricks</li></h3>
        </div>
    </div>

</div>
<style>
    
    .grid{
        display:grid;
        grid-template-columns:1fr 1fr 1fr;
        gap:30px;
    }

    .card{
        background:#333;
        overflow:hidden;
        height:240px;
        display:flex;      
        border-radius:20px;  
    }

    .image{
        width:30%;
        background-image:url('https://rickandmortyapi.com/api/character/avatar/119.jpeg');
        background-size:cover;
        background-position:center;
    }

    .info{
       padding: 10px, 20px, 15px, 20px;
    }
    :root{
        --main-colour: white;
    }

    .dead{
        background:firebrick;
        width:10px;
        height:10px;
        border-radius:100%;
        margin-right:10px;
    }

    .name{
        font-family:sans-serif;
        color:white;
    }

    .status{
        font-family:sans-serif;
        color: var(--main-colour);
        display:flex;
        align-items:center;
    }

    .locationLabel{
        color:#777;
        font-family:sans-serif;
        font-size:16px;
        margin:0 0 5px;        
    }

    .location{
        color:var(--main-colour);
        font-family:sans-serif;
        font-size:16px;
        display: flex;
        justify-content: center;
    }
</style>


