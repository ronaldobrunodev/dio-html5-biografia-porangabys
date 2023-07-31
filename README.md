# dio-html5-biografia-porangabys
Modelo de site simples em HTML 5


<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Porifólio">
    <meta name="keywords" content="HTML, CSS">
    <meta name="author" content="Ronaldo Bruno Cardoso">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">           
    <title>Biografia</title>
    <style>
        body{
            background-color: rgb(47, 6, 6);
            color: aquamarine;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: block;            
        }       
        header {
        text-align: center;
        background-image: linear-gradient(to right, #023047, #ffb703, #fb8500, #023047);
        padding: 1rem; 
        }
        .sobre{
            display: block;
            margin: -5px 20px;
            grid-column: auto; 
            padding: 1rem;  
        }
        table {
            padding: 0 auto;
            margin: 0 auto; 
            border-spacing: 3rem; 
        }
        td img {
            vertical-align: middle;
            border-radius: 100%;   
            border: solid 5px #fb8500; 
            height: 130px;
            width: 135px;            
        }
        td h1{
            margin-top: -39px;
            color: #023047;
            font-weight: bolder;
            font-size: 35px;            
        }
        td span{
            padding: 0;
            color: #023047;
            font-weight: bolder;
            font-size: 28px;
            text-decoration: #023047;
        }
        .grid-container {
        padding: 50px;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
        grid-gap: 50px; 
        margin: -5px 20px; 
        background-color: rgb(46, 52, 52);
        border-top-left-radius: 9px;
        border-top-right-radius: 9px;
        }
        .grid-container ul {
            padding: 5px;
            text-align: justify;
            display: flexbox;
            vertical-align: middle;            
        }
        form{
            vertical-align: middle;
            text-align: left;
            max-width: 100%;
        }              
        .endereco{                       
            margin: -5px 20px;
            max-width: 100%;
            max-height: max-content;
        }
        footer{
            text-align: center;   
            background-color: rgb(46, 52, 52);
            padding: 18px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));         
            margin: 0px 20px 0px ;
            background-color: rgb(46, 52, 52);       
            border-bottom-left-radius: 9px;
            border-bottom-right-radius: 9px;                   
        }  
        footer a{             
            text-align: center;   
            text-decoration: none;
            color: #ffb703;
        }
    </style>
</head>
<body>
    <header>
        <table cellspacing="0">
            <tr>
                <td><img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxMSEhUTEhIVFRUVFRUXFxUVFxUXFxc
                    VFRcXFxcXFRUYHSggGB0lHRUVITEhJSkrLi4uFx8zODMtNygtLisBCgoKDg0OFhAPFy0fHR0rLS0tLS0tLS0rKystLS0rKystLSs
                    tLSsrLS0tLS0tKystKy03LSstLS0tLTctLS03Lf/AABEIALcBEwMBIgACEQEDEQH/xAAcAAACAwEBAQEAAAAAAAAAAAABAgADBAU
                    GBwj/xAA7EAACAgEBBQUFBQcEAwAAAAAAAQIRAyEEEjFBUQUiYXGBBhMykaEHQrHR8BQjUmKCweEkNGNyc5Ky/8QAGgEBAQEBAQE
                    BAAAAAAAAAAAAAAECAwQFBv/EACIRAQEAAgIDAAMAAwAAAAAAAAABAhEDIRIxQQQTUSIy4f/aAAwDAQACEQMRAD8A+cEQQ0et4RS
                    JQUEAJEaGRGgM80JZZMraKgpjAUQoqBJFbLmhVACtGjFg5sMElwWviNG6/XyNzFnY7lDxgVvIkVuT8vD9cDSLnJLS/kUzlLilaGj
                    Q7Apjmd/DWpc4pkmKn+v7DRtXLGKjTFFWSBzuH8bmRYlkZFcUFo5tm3iWKojBEA4hslAJujxgFIhQKCiSREihkFAGAJCEAooZB3S
                    UQRkQ1ASKGRGGKI0QZpitFskSioRINDpEaKhGWKFglEaPEuKVN1C5J9BssimcqVL+x0ZR6efX8hkgYo9S9f4ASMA3w+Y7E6vpS8w
                    FYifIPqLJAPGV6MEnXkKuvQtpNcgEfgQXgxmc8sW8aKDQENZzaCghTIURIKQBolEaFSLUgSiQVjpASCgGogaIUVoNAQwCpDJEsMW
                    BEiSC5CsCiTDFBcS7HAJFcYB3SygUF0RxFmjRHGZdqbT1TrqaxrOUJKVCwhZIK/1+vE0bh0jARQ3ysi0A2wC3+v8AJWloHe5CuVA
                    AErDCXiSbArxumPB0/wAPyEYkshNi+TvQSL1oolkLNnjbvoS3pZO2mMSbo6JRydS7pGEiCAPFE3C7HGigRjQJljEaIKmhohSGooF
                    ACQCtDIiQ1AK0LRYxWgFQ1BolAK0NFjKIVAANjY42TcNGONEWA40W9m7Gs2WON/etJ9O63fpQmSR0vZfA55Zbr7yxT3fNuMfwk16
                    mMrqWuvHjLnIw9qdgShKXu6zQX3o6SXOpRb4+RxpwSdNyi+jT0+Z9L2bYPd4kpXvSuUr5PhX0R5TtrYJSk6/wZ4+e/XTl/Fku8Xn
                    pXykn5iuc1xja8NSzbNjcZbrpddKRmWKnV+qO/wCx5f1UZbYuaodTjIEsT635pMrlj6wX9Lr6FmcqXiynxckQohKP8cl4PUuSfJx
                    frRuVz0XKjMap3WsX6amSU6JViyENdTUmU4pbzNMImK3iVSHUiZICwRFM2RMDRdigQNjiO2SxQqWSxJMKAcjFbIioIA0QCIICWAG
                    QlBACQ1ESGACGiRjYFqCLMeMOUvK5Gdt6ZXFna9kdqWHaYuXCScH5umvql8zm0LIzlNzTWF8cpf4+i7a2nrpf9zkbbs16oHZGWeT
                    Z3Kcm3vNX4JJL+5amnxPJrV0+nuZzf9eX7S2Ry8Tn4eyJN3wR6rPCI+xQUk2uR0mbneLdeV7QwbqSo4+az1Ha+O5NnHls50xvTjn
                    h3pyo49deAyweGnXmdOGyF8dibNeblOJh2fY3LhKXzN+z7FiU6mpTaa4vTXimkdDZdmUUPn2ZRnLJOqSUklzXK+l6GLnb1t1w4cZ
                    3Y4vaGNRySjFaRe6v6dPxKVItlkt2+L1DKKO06jy5TdtZ94MCUNBFcxUC0iIwqWLJjWJJgKMiJBoIiCgDQRRAFlEAqQyFoZAGiUQ
                    IAIxgNALY+OVMSiMDZ7yyNmHfY8MjsmmttYGhhooyr1Xs/wD7aK/ml/8ATHyYtGyrsGE1hjvRajKUtxv71Ve74Jvj59GdLPFKNnj
                    z/wBq+nxd4R5zJilN0uHNnR2fao4qxvG00viq0359S/DngnVoq7QlvRdJoOm3I7Rywb0rU5GWG61zsszdnW+820aFsSqvxOvqOOW
                    7SRxpjS05iVWgYQt6mUrTjdK20vPTRHM7b7W981GCqKq3/E1z8jP21kvJS4RSXrxf4mFI7YYT3Xl5ea94w6L4spQ6OrhLUcdR4RA
                    kNYQGyWRgCJJgQGNFBTIgUghCsePL6+fh00oCQUihyAsIGeLGZUmNvAWxYxTZZFgEIoWALFkMxAFbJF6iyYEwOhvaF/ZcPfZ8WCP
                    HLkhC+ilJJteSt+hyZ5XwPZ/ZB2d73b3lfDBjbX/efcj9PefJEs62su7I9P24mtplhUKWODcFyhjhP3eKMfNQk/VeJytrzd3zPee
                    1fZrmlmhG5xTU4rjKGmsVzapadLPnm18b+638jxZTt9XC/wCLKtjxrvuUlLqm19OBm2qWaPw5JZF0b19VwZ1X2epx40cXbuyZR+D
                    I/IuNn1qzU6jNPa8r+LE2vRf3BHammrhKK8Vp8xXgzLi7XhQzyOqaN3XxzrQ4JqyjJkULk+Qcc3VGL2mxPBmjim7vFiyPSqeSO9T
                    60mhjhbXLkz8ZtycmRybk+LbfzImWuKDCJ6Hj1ssSxIlDpjaaVg3ixiqBTSRVjNESGIaVuBEPQKKaRMaxUPGINIhiJEoJYO6QKAB
                    jsiBYYlZMi1MrRFIKuSICLI4MFCRUy5QJOKRdJtnA2Gb1FZQEz6n9iqUY53zc18ktPrZ8qPS+wHtJ+ybTuzf7qbp/yt1TF7i4XWU
                    r75lmeW9oewYZrnBqGTy7s3/MlwfivVM9DDImk07TWjXRlO0Y7ONxl9vbMrPT5RtuTLge5OLT5eK6xfBo58u0V94+l9pbAskXGa3
                    o9H+K6PxPE9q+y8428L3l/DLj6S5+vzOf646ftrkx7TRVkm58OHUp/ZJQlWSLi+klT9PDxRt2LY55Ze7wwc5Ok3yX/aXL8SeMPK3
                    22+z/AGT7/JDElpLXJL+HEvi8t7SK8/A5X2rxrtBvhvYcb08N6K+kUfW/Z7sKOyYd296ctck6+KXKukVyX5nyf7Xn/rYP/hS+UpP
                    +5245p5+e7xeQxZ60eqOhjmmrRyZMfFko6XHbzTLTqtBaMsM5dHP1RPGr5yrYoDAsifMNGa1A3g7xN0CQU28RiBADLIsUIRZvA3h
                    AhKeyCJEKjIiyC6DpLoWQZvTOwWPqFY0MpERdIZaCtksVyCJZVOYubIVwALEbLGiqaI0FlOR6+g030KZqmVmvr/2Z+1m/COz5XrH
                    RSfLXu+juvBrx0+h5Ufm7sLtD3GaGR6xTqa6wfFefNeKR+gOxNvjkShvb1wUsc+O9Brr1X1Xqc8p9enhz3NVfkhZn/ZbZ0pYGea9
                    vO3v2LBUNc2TSCVXFcJT16cvGvEy63p5z2n9pcMc3uFjWWMHUu5Ga95/Cr6eHO+hj2X23yYcsPd7NcIPdnhUFB6vXcrhLThz+p41
                    7Vv05O9NUr0eqW91fP1Nyn3YyjjlG+D4JuPHXh+RdMb39fc4bbDNjhlxy3oTipRfg+vR+B8R+1l/6yC/419ZM9n9l/am8suzy4KT
                    y4k6+Fvvx00u6l470meA+07Pvbfl/k3I/JW/rI1Jpnku8Xm5x0Fiy6PAonGmbeaHhko0xnZisbFkryEq2N1hjkK4yJI0wv9+wrOZ
                    2yqT1VGbjGvOtvvSLKUUFROdkbmV0074YzKEEaXyrQpkcygNDR5Ld8hXTIXTO0xyGb5mdMshI2yt3hoMzpjwYF1gySAmVud6AVJW
                    y1giqDL9UFgNiMkpoTiRbSqPMrzovoTItGVzURPqf2U9q+8hLZ2173Et7FfOLdteNO1/UkfLEdHsLtOWzZ8eeN3CSbS5x+8vVEs3
                    GsMvG7fpDL2lCGD30ulbq4ufDdXjf5nz3a9iltGWWbKt6UuXJRXCK8PzbPZQjh2uMcmOu+lJPlJNLXwdUDHsKV6VXG+Rzl091m3y
                    rt/2Vlg3p4e8pK1HmvGP4UcfFj3cSlJTe9LcjVVvV3tN61y4x/wAe69stsqDqSg5d2EXxcb7zS9efU8R2njWNY3jbTU1b4NOmnre
                    qTcdfEWs+Ot19O9iuzcbwPNGt9y7kv4WuT5rjTXRnxj2pzvJtOebu3km6fLXgz2/sx2k9knGXvP3eTTJFu6V0pSSXdkm16NniPaP
                    /AHGb/wAk39S497c+WakYsT0JJdRdm4Fh0jzX2zzhQywsvoDWo0uxhwDHxIBcTTJiuf5DMTIQX4Hqad0x43qjWmc8/brx+hcRVEL
                    ZEzLVRjJitEiisrCCkAztUSDGnErOjC2TGgyq+QimBrsz5ZU0W4plWfiFW8RZAxPkWboRWmFKgyRIgChJj2I0EZ0uIUyS4+YpB9d
                    +xbt2Mt7ZMj70bnivnH70V5N3/V4Hv+1FWXT4Zx3fXgfnDsntCez5sebH8WOSkvHrF+DVr1PvOw9oR2nZFlxu9VJdUua9Gc8se9v
                    Vw57mnifbzaoe/nj540o8VWsVL4ety49EeXh7meXdbmouCT5u9N5pKr11rwZr9r9sT2vNKkv307knb0e6rXKt36HG2jJCU4XFyja
                    uMZb0qrvU/F6158CR0task8aW48k3uyx1GXNO9/ed91pV82cLtZp5MjTvvS1qufTkdLB7v3M7u9W+D6/E/wD1rxs4ebnx9dX8zWL
                    jy3qBsr4o0JGXZuJrZuenC+ysDfQaiJFZRREg9SyQN3mURleR6DyEyLRgGLNkXoYos1YnoZynTeF7XEFbHx4nK6XDic3bW0TCyOL
                    XILxy40xtmwKIDeCVFbRnyKiEOjmEZC5OJCEVds/AOTUJAColsXYSFCyRXZCBKAJEIEU5l+IhCAQ979l/tCsEsmGbbjLHKUEr+Jf
                    EvC1r6PqQhL6bwuso8v2ltjyydcW5aUlxk5O3z1KsOdKbuCVpd1N1VdeXJ+gSHJ6N/WbLmhJSTTcm4tSvRJfFa526MeYhDpPThld
                    1VifeNpCFjOQUREIVkMjLIcCEKFcSqa0ZCEQIsvxS1AQfFnt672S7GhtF76upVXDlZ3e0tjw4u5DHUUrpa8n14kIfC5s8r+Rcd9P
                    1H43HhPxZlJN3/rysYKc6Ue7F35pas1bZtEFFprjpX+SEPdreUj5tusLZ9cBohCHrfPf/2Q==" 
                    alt="Foto: Ronaldo Bruno Cardoso"></td>
                <td><h1>VAL PORANGABYS</h1>
                <span>Engeheiro de Software</span></td>               
            </tr>
        </table>
    </header>    
    <main>
        <section   class="sobre">
            <h2>Sobre Mim</h2>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis vero, quia, provident maxime illum corrupti qui natus sit minima accusantium veniam temporibus accusamus soluta voluptatibus dolore porro tempora laudantium? Alias.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos numquam magnam est recusandae, perspiciatis, amet dicta voluptate tenetur a beatae error iste officiis aliquam pariatur autem! Omnis porro provident dignissimos.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis officiis accusantium doloremque? Mollitia, tempora! Tenetur voluptas quod corrupti hic earum animi temporibus ratione quis! Mollitia incidunt saepe voluptas placeat debitis?
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus accusamus excepturi laborum at nemo saepe sapiente. Hic quibusdam necessitatibus dicta, adipisci, tempora ipsa excepturi fuga sunt quam eius odit assumenda?
            </p>            
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis vero, quia, provident maxime illum corrupti qui natus sit minima accusantium veniam temporibus accusamus soluta voluptatibus dolore porro tempora laudantium? Alias.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos numquam magnam est recusandae, perspiciatis, amet dicta voluptate tenetur a beatae error iste officiis aliquam pariatur autem! Omnis porro provident dignissimos.
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis officiis accusantium doloremque? Mollitia, tempora! Tenetur voluptas quod corrupti hic earum animi temporibus ratione quis! Mollitia incidunt saepe voluptas placeat debitis?
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus accusamus excepturi laborum at nemo saepe sapiente. Hic quibusdam necessitatibus dicta, adipisci, tempora ipsa excepturi fuga sunt quam eius odit assumenda?
            </p>
        </section>
        <section class="grid-container">
            <section>
            <h2>Experiência Profissional</h2>
            <ul>
                <li>
                    <strong>Nome da Empresa</strong> - Cargo ocupado (Data de início - Data de saída)
                    <p>Descrição das responsabilidades e conquistas no cargo.</p>
                </li>                
            </ul>
        </section>
        <section>
            <h2>Formação Acadêmica</h2>
            <ul>
                <li>
                    <strong>Nome da Instituição</strong> - Curso (Data de início - Data de conclusão)
                </li>               
            </ul>
        </section>
        <section>
            <h2>Conquistas e Prêmios</h2>
            <ul>
                <li>Descrição de conquistas e prêmios relevantes.</li>               
            </ul>
        </section>
        <section>
            <h2>Hobbies e Interesses</h2>
            <ul>
                <li>Lista de hobbies e interesses pessoais.</li>                
            </ul>            
        </section>
        <section>
            <h2>Siga-nos</h2>
            <iconify-icon icon="skill-icons:instagram"></iconify-icon>
            <iconify-icon icon="devicon:facebook"></iconify-icon>
            <iconify-icon icon="devicon:linkedin"></iconify-icon>
            <iconify-icon icon="logos:github-octocat"></iconify-icon>
            <iconify-icon icon="logos:telegram"></iconify-icon>
            <iconify-icon icon="logos:youtube-icon"></iconify-icon>
            <h2>Endereço</h2>
            Curitiba, Paraná-BR <br />
            CEP: 8520-000
        </section>
        <section>
            <h2>Contato</h2>
            <form action="/enviar_contato" method="post">               
                <input type="text" id="nome" name="nome" required placeholder="Nome"> <br /> 
                <input type="email" id="email" name="email" required placeholder="E-mail"><br />                
                <label for="mensagem">Mensagem:</label> <br />
                <textarea id="mensagem" name="mensagem" required placeholder="Escreva aqui sua mensagem"></textarea> <br />                
                <button type="submit">Enviar</button>
            </form>
        </section>        
    </section>
    <section class="endereco">       
        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d230483.82329555397!2d-49.45461475820938!3d-25.494714567360134!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94dce35351cdb3dd%3A0x6d2f6ba5bacbe809!2sCuritiba%2C%20PR!5e0!3m2!1spt-BR!2sbr!4v1690798767082!5m2!1spt-BR!2sbr" width="100%" height="200px" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </section>
    </main>   
    <footer>
        <p>Developer by: <a href="#">Ronaldo</a></p>
    </footer>
    <script src="https://code.iconify.design/iconify-icon/1.0.7/iconify-icon.min.js"></script>
</body>
</html>
