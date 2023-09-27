<script>
    import Header from "../components/Header.svelte";
    import Activity from "../components/Activity.svelte";
    import Footer from "../components/Footer.svelte";
</script>

<Header />
<main>
    <div class="main-view">
        <div class="column">
            <div class="catch-copy">
                <h1>テクノロジーと<br />ハンドメイドで<br/>世の中を豊かにする</h1>
            </div>
        </div>
        <div class="column">
            <div class="activities">
                <Activity titleText="技術書執筆" explainText="同人技術書を執筆して、世の中のトレンド技術の情報発信を行っています。" />
                <Activity titleText="ハッカソン" explainText="各種ハッカソンに参加して、世の中に「新しくて面白い」を届けます。" />
                <Activity titleText="ハンドメイド作品販売" explainText="ハンドメイドアクセサリー・ハンドメイド雑貨など、一点ものの服飾品を製作・販売しています。" />
            </div>
        </div>
    </div>
    <div class="sub-view">
        <div class="column">
            <img class="thumbnail" src="thumb.jpg" alt="thumbnail" />
        </div>
            <div class="column">
                <div class="profiles">
                    <div class="profile-title">
                        <h2>Member</h2>
                    </div>
                    <p class="profile">Name:れいじ</p>
                    <p class="profile">X:@reiji1020</p>
                    <p class="profile">Circle Owner/Web Developer/Handmade Creator</p>
                </div>
            </div>
    </div>
</main>
<Footer />

<style>
    h1 {
        font-size: 48px;
        color: #ED3B7D;
    }

    h2 {
        font-size: 32px;
        color: #FFF;
        margin: 0;
    }

    .main-view {
        height: 450px;
        background: linear-gradient(180deg, rgba(237, 145, 38, 0.50) 50%, rgba(255, 255, 255, 0.00) 100%);
        display: flex;
    }
    .column {
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .activities {
        display: flex;
        flex-direction: column;
        width: 768px;
    }

    .sub-view {
        height: 400px;
        background: rgba(32, 137, 234, 0.50);
        display: flex;
    }

    .profiles {
        display: flex;
        flex-direction: column;
        width: 768px;
    }

    .thumbnail {
        width: 256px;
        height: 256px;
        border-radius: 50px;
    }

    .profile-title {
        border-radius: 27.5px;
        background: #2089EA;
        width: 250px;
        height: 60px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .profile {
        color: #4B4B4B;
        font-size: 24px;
        font-weight: 700;
    }
</style>