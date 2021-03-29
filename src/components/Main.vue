<template>
    <main>
        <div class="main">
            <p class="first-view">これから実務経験を積みたい人はいっぱいいると思いますが「何を勉強すればいいんだろう」と思う人がいっぱいいると思います。<br>私は2020年からコーダーとして実務を始めましたが私が実務を始めるまでにした勉強について説明します。</p><!--/.first-view-->
            <section id="lesson">
                <div class="lesson">
                    <ul class="lesson-flexbox">
                        <li 
                            v-for="list in lists"
                            :key="list.id"
                            class="list"
                        >
                            <h2>{{list.title}}</h2>
                            <p class="content">{{list.content1}}<br>{{list.content2}}<br>{{list.content3}}<span>{{list.span}}</span><br>{{list.content4}}<br>{{list.content5}}</p><!--/.content-->
                        </li>
                        <li 
                            v-for="list in lists1"
                            :key="list.id"
                            class="list"
                        >
                            <h2>{{list.title}}</h2>
                            <p class="content">{{list.content1}}<span>{{list.span}}</span>{{list.content2}}<br>{{list.content3}}<br>{{list.content4}}<br>{{list.content5}}<br>{{list.content6}}</p><!--/.content-->
                        </li>
                    </ul><!--/.lesson-flexbox-->
                </div><!--/.lesson-->
            </section><!--/.lesson-->
            <section id="last">
                <h2>最後に</h2>
                <p class="last-content">コーディング自体は<span>思った以上に難しくない</span>です！<br>コーディングで凄く大事なのは見た目が整っていることです。<br>それも私のコミュニティでは身につけることができる様にしますのでコーディングを頑張りましょう。</p><!--/.last-content-->
            </section><!--/.last-->
        </div><!--/.main-->
    </main>
</template>

<script>
    export default{
        data:function(){
            return{
                lists:[
                    {
                        title:'1、まずはProgate!',
                        content1:'私もですがまずはProgateのHTMLとCSSのコースから始めた方が挫折しないと思います。',
                        content2:'全部できないといけないと思うかもしれませんがそうでもないです！',
                        content3:'実務では',
                        span:'使わない内容が結構あります。',
                        content4:'例えばfloatプロパティ、私が実務を始めて1度も使っていません 笑',
                        content5:'だから「全部覚えないと」って考えるとプレッシャーになるから「使えるようにしよう」位に考えた方がいいです。'
                    },
                ],
                lists1:[
                    {
                        title:'2、次はサイトの模写だけど、、',
                        content1:'サイトによってコーディングの難易度が違うから',
                        span:'これが凄く大変',
                        content2:'です、、',
                        content3:'ネットを見るとオススメがサイトによって違ってどれを使えばいいか分からない、、',
                        content4:'でも大丈夫です！',
                        content5:'私のコミュニティでは私が勉強していた時に苦労した経験を元にこういう順番でコーディングをすればいいというデザインカンプを作ります。',
                        content6:'それと実務でデザインカンプに指示が付いている時もあるのですがそれも付けて練習して実務に近い形に持っていきます！'
                    }
                ],
            }
        }
    }
</script>