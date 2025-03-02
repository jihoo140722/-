/* 기본 스타일 설정 */
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background-color: #000;
    color: #fff;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    overflow: hidden;
}

/* 보석 표시 */
#gemDisplay {
    font-size: 18px;
    margin-bottom: 20px;
    padding: 10px;
    background-color: rgba(50, 50, 50, 0.7);
    border-radius: 10px;
}

/* 게임 화면 설정 */
#gameCanvas {
    border: 2px solid #fff;
    background-color: #000;
    margin-bottom: 20px;
}

/* 버튼 스타일 설정 */
button {
    background-color: #444;
    color: #fff;
    border: none;
    padding: 10px 20px;
    margin: 10px;
    cursor: pointer;
    border-radius: 5px;
}

button:hover {
    background-color: #666;
}

/* 소리 설정 버튼 스타일 */
#soundButton {
    position: absolute;
    top: 20px;
    left: 20px;
}

/* 언어 설정 버튼 스타일 */
#languageButton {
    position: absolute;
    top: 20px;
    right: 20px;
}

/* 아이템 상점 스타일 */
#itemShop {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    width: 90%;
    max-width: 600px;
    background-color: rgba(50, 50, 50, 0.9);
    padding: 15px;
    border-radius: 10px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    box-shadow: 0px 0px 15px rgba(255, 255, 255, 0.5);
}

/* 자동차 아이템 스타일 */
.car-item {
    width: 120px;
    padding: 10px;
    text-align: center;
    background-color: #222;
    border-radius: 8px;
    margin: 10px;
    transition: transform 0.3s ease;
}

.car-item:hover {
    transform: scale(1.1);
    background-color: #333;
}

.car-item img {
    width: 100px;
    height: 60px;
    object-fit: cover;
    border-radius: 5px;
}

/* 구매 버튼 스타일 */
.buy-button {
    background-color: #0084ff;
    padding: 5px;
    margin-top: 5px;
    font-size: 14px;
    border-radius: 5px;
}

.buy-button:hover {
    background-color: #005fcc;
}

/* 자동차 선택 영역 */
#carSelect {
    margin-top: 20px;
    padding: 10px;
    background-color: rgba(50, 50, 50, 0.8);
    border-radius: 10px;
    display: flex;
    justify-content: center;
    gap: 10px;
}

/* 자동차 선택 버튼 */
#carSelect button {
    padding: 5px 15px;
    background-color: #222;
    color: #fff;
    border: none;
    cursor: pointer;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

#carSelect button:hover {
    background-color: #444;
}

/* 반응형 디자인 */
@media (max-width: 768px) {
    body {
        padding: 10px;
    }

    #itemShop {
        width: 100%;
    }

    .car-item {
        width: 100px;
        padding: 8px;
    }
    
    #carSelect {
        flex-direction: column;
        align-items: center;
    }
}
