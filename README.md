# melody_cinematics
<!doctype html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM"
        crossorigin="anonymous"></script>

    <title>8팀 멜로디 시네마틱스 | 자기소개 페이지</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Gowun+Dodum&display=swap');

        * {
            font-family: 'Gowun Dodum', sans-serif;
        }

        .mytitle {
            background-color: white;
            color: white;
            height: 250px;

            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;

            background-image: linear-gradient(0deg, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("https://i.ytimg.com/vi/UuSHFD1lOrs/hqdefault.jpg");
            background-position: center;
            background-size: cover;

        }

        .mytitle>button {
            width: 250px;
            height: 50px;
            background-color: transparent;
            border: 1px solid white;
            color: white;
            border-radius: 50px;
            margin-top: 20px;
        }

        .mytitle>button:hover {
            border: 2px solid white;
        }

        .mycomment {
            color: gray;
        }

        .mycards {
            width: 800px;
            margin: 10px auto 10px auto;
        }

        .mypost {
            background-color: white;
            width: 500px;
            margin: 20px auto 20px auto;
            padding: 20px 20px 20px 20px;
            box-shadow: 0px 0px 3px 0px gray;

        }

        .mybtn {
            display: flex;
            flex-direction: row;
            align-items: center;
            justify-content: center;

            margin-top: 20px;

        }

        .mybtn>button {
            margin-right: 10px;
        }
    </style>
    <script>
        $(document).ready(function () {
            fetch("http://spartacodingclub.shop/sparta_api/weather/seoul").then(res => res.json()).then(data => {
                let number = data['temp']
                $('#temp').text(number)
            })

        })

    </script>
    <script>
        function hey(){
            alert('8팀에 오신것을 환영합니다!')
        }
    </script>
</head>

<body>
    <div class="mytitle">
        <h1> 8팀 멜로디 시네마틱스  </h1>
        <h2> 자기소개 페이지 </h2>
        <button onclick="hey()"> 나를 누르시오
    </div>
    <div class="mypost">
        <div class="form-floating mb-3">
            <input type="email" class="form-control" id="floatingInput" placeholder="name@example.com">
            <label for="floatingInput">나를 대표하는 이미지 URL</label>
        </div>
        <div class="input-group mb-3">
            <label class="input-group-text" for="inputGroupSelect01">Options</label>
            <select class="form-select" id="inputGroupSelect01">
                <option selected>나를 나타내는 아이콘</option>
                <option value="1">🐿️</option>
                <option value="2">🧚🏻</option>
                <option value="3">👽</option>
                <option value="3">👻</option>
                <option value="3">👨🏻‍🍳</option>
                <option value="3">🥷🏼</option>
                <option value="3">👼🏻</option>
                <option value="3">🕺🏻</option>
                <option value="3">🦄</option>
                <option value="3">🐜</option>
            </select>
        </div>

        <div class="form-floating">
            <textarea class="form-control" placeholder="Leave a comment here" id="floatingTextarea"></textarea>
            <label for="floatingTextarea">나를 한줄로 소개하기</label>
        </div>
        <div class="mybtn">
            <button type="button" class="btn btn-dark">기록하기</button>
            <button type="button" class="btn btn-outline-dark">닫기</button>
        </div>

    </div>
    <div class="mycards">
        <div id="cards" class="row row-cols-1 row-cols-md-3 g-4">
            <div class="col">
                <div class="card h-100">
                    <img src="https://movie-phinf.pstatic.net/20210728_221/1627440327667GyoYj_JPEG/movie_image.jpg"
                        class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">이름이 들어갑니다.</h5>
                        <p class="card-text">나를 한줄로 소개한다면?</p>
                        <p> 🐙 내 이모티콘</p>
                        <p class="mycomment">TMI 대방출~~~롤로랄라</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100">
                    <img src="https://movie-phinf.pstatic.net/20210728_221/1627440327667GyoYj_JPEG/movie_image.jpg"
                        class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">이름이 들어갑니다.</h5>
                        <p class="card-text">나를 한줄로 소개한다면?</p>
                        <p> 🐙 내 이모티콘</p>
                        <p class="mycomment">TMI 대방출~~~롤로랄라</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100">
                    <img src="https://movie-phinf.pstatic.net/20210728_221/1627440327667GyoYj_JPEG/movie_image.jpg"
                        class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">이름이 들어갑니다.</h5>
                        <p class="card-text">나를 한줄로 소개한다면?</p>
                        <p> 🐙 내 이모티콘</p>
                        <p class="mycomment">TMI 대방출~~~롤로랄라</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card h-100">
                    <img src="https://movie-phinf.pstatic.net/20210728_221/1627440327667GyoYj_JPEG/movie_image.jpg"
                        class="card-img-top" alt="...">
                    <div class="card-body">
                        <h5 class="card-title">이름이 들어갑니다.</h5>
                        <p class="card-text">나를 한줄로 소개한다면?</p>
                        <p> 🐙 내 이모티콘</p>
                        <p class="mycomment">TMI 대방출~~~롤로랄라</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>

</html>
