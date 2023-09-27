<script lang="ts">
    /**
     * メインビュー内で使用する活動内容説明用コンポーネント
     * */
    export let titleText: string /* タイトル文字列 */
    export let explainText: string /* 説明文 */

</script>

<div class="activity">
    <div class="title">
        <h2>{titleText}</h2>
    </div>
    <div class="explain">
        <p>{explainText}</p>
    </div>
</div>

<style>
    h2 {
        font-size: 32px;
        color: #FFF;
        margin: 0;
    }

    p {
        margin: 12px 0;
    }

    .activity {
        display: flex;
        flex-direction: column;
    }

    .title {
        border-radius: 27.5px;
        background: #ED3B7D;
        width: fit-content;
        padding: 4px 16px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .explain {
        font-size: 20px;
        color: #4B4B4B;
        margin: 0 16px;
    }
</style>