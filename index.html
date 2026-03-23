<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <title>プロフィール自動作成</title>
    <link rel="shortcut icon" href="https://mixch.tv/favicon.ico">
    <meta name="description" content="スキマ時間で完成。コピペするだけのミクチャ最強プロフィール生成ツール。">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        /* --- 基本設定 --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(135deg, #667eea, #f093fb);
            font-family: 'Hiragino Kaku Gothic Pro', Meiryo, 'MS PGothic', sans-serif;
            font-size: 12px;
            line-height: 1.4;
            letter-spacing: 0.05em;
            color: #3c3c3c;
            min-height: 100vh;
        }

        /* --- レイアウト --- */
        .container {
            max-width: 480px;
            margin: 0 auto;
            padding: 20px 0;
        }

        .content-card {
            background-color: #fff;
            width: 95%;
            margin: 0 auto;
            border-radius: 20px;
            padding: 20px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }

        header {
            text-align: center;
            margin-bottom: 25px;
            padding-bottom: 20px;
            border-bottom: 3px solid #e0e0ff;
        }

        .title {
            font-size: 22px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 50%, #f093fb 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 8px;
            font-weight: 900;
        }

        header p {
            font-size: 13px;
            color: #666;
            font-weight: 500;
        }

        /* --- フォーム関連 --- */
        .form-section {
            margin-bottom: 25px;
            padding: 15px;
            background: linear-gradient(135deg, #f8f9ff 0%, #fff5f8 100%);
            border-radius: 18px;
            border: 2px solid #e0e0ff;
        }

        .form-section h3 {
            font-size: 16px;
            color: #667eea;
            margin-bottom: 15px;
            font-weight: 800;
        }

        .form-group {
            margin-bottom: 18px;
        }

        .form-group label {
            display: block;
            font-weight: 700;
            margin-bottom: 6px;
            color: #667eea;
            font-size: 13px;
        }

        .label-flex {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 6px;
        }

        .label-flex label { margin-bottom: 0 !important; }

        .required {
            background: #ff4757;
            color: white;
            padding: 2px 6px;
            border-radius: 8px;
            font-size: 10px;
            margin-left: 5px;
        }

        input, textarea, select {
            width: 100%;
            padding: 12px;
            border: 2px solid #e0e0ff;
            border-radius: 10px;
            font-size: 16px;
            transition: all 0.3s ease;
            font-family: inherit;
            background: white;
            color: #333;
        }

        input::placeholder, textarea::placeholder { font-size: 12px; }
        textarea { resize: vertical; min-height: 70px; }

        .random-phrase-btn {
            margin-top: 8px;
            background: #667eea;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 8px;
            font-size: 12px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.2s;
        }

        .random-phrase-btn:hover { background: #764ba2; }

        /* --- モーダル --- */
        .modal-checkbox { display: none; }
        
        .modal-open-button {
            color: white;
            padding: 2px 10px;
            cursor: pointer;
            font-weight: bold;
            font-size: 10px;
            letter-spacing: 1px;
            background-color: #FF0088;
            border-radius: 50px;
            line-height: 1.8;
        }

        .modal {
            position: fixed;
            inset: 0;
            z-index: 9999;
            display: none;
            align-items: center;
            justify-content: center;
            background-color: rgba(0, 0, 0, 0.6);
        }

        .modal-checkbox:checked + .modal { display: flex; }

        .modal-wrapper {
            position: relative;
            width: 85%;
            max-width: 400px;
            padding: 20px 0;
            background-color: #FEFEFE;
            border-radius: 15px;
            border: 2px solid #FF0088;
        }

        .close {
            position: absolute;
            top: 10px;
            right: 15px;
            font-size: 24px;
            cursor: pointer;
        }

        .modal-wrapper .head {
            font-size: 18px;
            padding: 10px;
            font-weight: bold;
            text-align: center;
        }

        .modal-wrapper .text {
            width: 85%;
            margin: 0 auto;
            font-size: 12px;
            border-radius: 12px;
            padding: 15px;
            background-color: #FFE9F4;
            line-height: 1.6;
        }

        .point {
            background-color: #FF0088;
            width: fit-content;
            margin: 0 auto;
            color: white;
            padding: 4px 15px;
            border-radius: 50px;
            font-size: 11px;
            font-weight: bold;
        }

        .pink { font-weight: bold; color: #FF0088; }

        /* --- 生成結果エリア --- */
        .result-container {
            margin-top: 30px;
            padding-top: 25px;
            border-top: 3px solid #e0e0ff;
        }

        .profile-output {
            width: 100%;
            padding: 15px;
            background: #f9f9ff;
            border-radius: 15px;
            border: 2px dashed #667eea;
            min-height: 150px;
            white-space: pre-wrap;
            word-wrap: break-word;
            line-height: 1.5;
            font-size: 14px;
            color: #333;
        }

        /* --- ボタン・トースト --- */
        .button-group {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
            margin: 20px 0 10px;
        }

        .copy-btn, .mixchannel-btn {
            padding: 14px 10px;
            border: none;
            border-radius: 12px;
            font-size: 13px;
            font-weight: 800;
            cursor: pointer;
            color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .copy-btn { background: linear-gradient(135deg, #10b981, #059669); }
        .mixchannel-btn { background: linear-gradient(135deg, #FF6B9D, #C44569); }

        .os-label {
            font-size: 10px;
            background: rgba(255,255,255,0.2);
            padding: 2px 8px;
            border-radius: 4px;
            margin-bottom: 5px;
        }

        .reset-btn { 
            background: #eee; 
            color: #666;
            width: 100%;
            padding: 12px;
            border-radius: 10px;
            border: none;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
        }

        .toast {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%) translateY(100px);
            background: #333;
            color: white;
            padding: 12px 24px;
            border-radius: 50px;
            font-size: 14px;
            transition: 0.3s;
            z-index: 4000;
            opacity: 0;
        }

        .toast.show {
            opacity: 1;
            transform: translateX(-50%) translateY(0);
        }
    </style>
</head>
<body>

<div class="container">
    <div class="content-card">
        <header>
            <h1 class="title">🎤 ミクチャプロフィール<br>AI生成</h1>
            <p>あなたらしいプロフィールを自動作成</p>
            <div style="font-size:12px;color:#888;margin-top:4px;">※入力すると下に自動で反映されます</div>
        </header>

        <form id="profileForm">
            <div class="form-section">
                <h3>👤 <ruby>基<rt>き</rt>本<rt>ほん</rt>情<rt>じょう</rt>報<rt>ほう</rt></ruby></h3>
                <div class="form-group">
                    <label for="name">お<ruby>名<rt>な</rt>前<rt>まえ</rt></ruby> <span class="required">必須</span></label>
                    <input type="text" id="name" placeholder="例：お名前＋ファンマーク(本名じゃなくてOK)">
                </div>
                <div class="form-group">
                    <label for="furigana">ふりがな</label>
                    <input type="text" id="furigana" placeholder="例：おなまえ">
                </div>
                <div class="form-group">
                    <label for="catchphrase">キャッチフレーズ</label>
                    <textarea id="catchphrase" rows="2" placeholder="例：私の成長を見届けてください！"></textarea>
                    <button type="button" class="random-phrase-btn" id="randomPhraseBtn">🪄 AIでランダム生成</button>
                </div>
            </div>

            <div class="form-section">
                <h3>🎉 イベント &amp; <ruby>配<rt>はい</rt>信<rt>しん</rt>情<rt>じょう</rt>報<rt>ほう</rt></ruby></h3>
                <div class="form-group">
                    <label for="currentEvent">参加するイベント名</label>
                    <select id="currentEvent">
                        <option value="">選択してください</option>
                        <option value="月刊わんこ掲載モデルオーディション">月刊わんこ掲載モデルオーディション</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="eventGoal">イベント<ruby>目<rt>もく</rt>標<rt>ひょう</rt></ruby></label>
                    <input type="text" id="eventGoal" placeholder="例：初めての1位獲得！">
                </div>
                <div class="form-group">
                    <div class="label-flex">
                        <label for="streamSchedule">自分が<ruby>配<rt>はい</rt>信<rt>しん</rt></ruby>する日時</label>
                        <label for="modalToggle1" class="modal-open-button">CHECK!</label>
                    </div>
                    <input type="checkbox" id="modalToggle1" class="modal-checkbox">
                    <div class="modal">
                        <div class="modal-wrapper">
                            <label for="modalToggle1" class="close">&times;</label>
                            <div class="point">ONE POINT</div>
                            <div class="head">🌟 配信時間のコツ</div>
                            <div class="text">
                                不定期の場合は告知先が分かるように<br>
                                <span class="pink">「Xまたはストーリーで告知するので、チェックお願いします！」</span><br>
                                のように記載しましょう！
                            </div>
                        </div>
                    </div>
                    <textarea id="streamSchedule" rows="2" placeholder="例：基本毎日21:00〜配信！"></textarea>
                </div>
                <div class="form-group">
                    <label for="content">MBTI(あれば)</label>
                    <input type="text" id="content" placeholder="例：INFP">
                </div>
                <div class="form-group">
                    <label for="awards"><ruby>受<rt>じゅ</rt>賞<rt>しょう</rt>歴<rt>れき</rt></ruby></label>
                    <textarea id="awards" rows="2" placeholder="例：CAMPUS BOYS 2025　ファイナリスト"></textarea>
                </div>
            </div>

            <div class="form-section">
                <h3>🌟 あなたについて</h3>
                <div class="form-group">
                    <div class="label-flex">
                        <label for="fanMark">ファンマーク</label>
                        <label for="modalToggle2" class="modal-open-button">CHECK!</label>
                    </div>
                    <input type="checkbox" id="modalToggle2" class="modal-checkbox">
                    <div class="modal">
                        <div class="modal-wrapper">
                            <label for="modalToggle2" class="close">&times;</label>
                            <div class="point">ONE POINT</div>
                            <div class="head">💎 ファンマークとは</div>
                            <div class="text">
                                好きな<span class="pink">絵文字2つ</span>設定してみてください！<br>
                                悩むときは配信でリスナーさんと相談して決めてもOK！！
                            </div>
                        </div>
                    </div>
                    <input type="text" id="fanMark" placeholder="例：🌸🌹">
                </div>
                <div class="form-group">
                    <div class="label-flex">
                        <label for="dream"><ruby>夢<rt>ゆめ</rt></ruby>・<ruby>目<rt>標<rt>ひょう</rt></ruby></label>
                        <label for="modalToggle3" class="modal-open-button">CHECK!</label>
                    </div>
                    <input type="checkbox" id="modalToggle3" class="modal-checkbox">
                    <div class="modal">
                        <div class="modal-wrapper">
                            <label for="modalToggle3" class="close">&times;</label>
                            <div class="point">ONE POINT</div>
                            <div class="head">🚀 目標の書き方</div>
                            <div class="text">
                                「有名になりたい」などの抽象的な言葉よりも、<br>
                                <span class="pink">具体的に○○になりたい！</span>と書くことで、熱いファンが付きやすくなります！<br><br>
                                コンテストにちなんだ目標だと、より熱量が伝わります！
                            </div>
                        </div>
                    </div>
                    <textarea id="dream" rows="2" placeholder="例：本気でモデルを目指してます！"></textarea>
                </div>
                <div class="form-group">
                    <label for="message">ファンへのメッセージ</label>
                    <textarea id="message" rows="2" placeholder="例：初心者ですが、よろしくお願いします！"></textarea>
                </div>
            </div>
        </form>

        <div id="result" class="result-container">
            <h2 style="font-size: 18px; margin-bottom: 15px; color: #667eea;"><ruby>生<rt>せい</rt>成<rt>せい</rt></ruby>結果</h2>
            <div id="profileOutput" class="profile-output">お名前を入力すると自動生成されます</div>
        </div>

        <div style="margin-top:30px; padding-top:20px; border-top:3px solid #e0e0ff">
            <h3 style="font-size:16px; text-align: center; color:#667eea; margin-bottom:20px;">✨使い方はかんたん！ 2ステップ✨</h3>
            <div style="display: flex; gap: 10px; justify-content: space-between; margin-bottom:20px;">
                <div style="flex: 1; text-align: center;">
                    <div style="background: #f0f0ff; border-radius: 10px; padding: 10px; margin-bottom: 8px; border: 1px solid #e0e0ff;">
                        <img src="https://github.com/iwakurashiori1008/other/blob/main/profile_1_.png?raw=true" alt="マイページ" style="width: 100%; border-radius: 5px;">
                    </div>
                    <p style="font-size: 11px; font-weight: bold; color: #666;">① ボタンから飛んで<br>「プロフィール」を選択</p>
                </div>
                <div style="display: flex; align-items: center; color: #e0e0ff; font-weight: bold;">▶︎</div>
                <div style="flex: 1; text-align: center;">
                    <div style="background: #f0f0ff; border-radius: 10px; padding: 10px; margin-bottom: 8px; border: 1px solid #e0e0ff;">
                        <img src="https://github.com/iwakurashiori1008/other/blob/main/profile_2_.png?raw=true" alt="自己紹介編集" style="width: 100%; border-radius: 5px;">
                    </div>
                    <p style="font-size: 11px; font-weight: bold; color: #666;">② 自己紹介欄に<br>貼り付けるだけ！</p>
                    <p style="font-size:9px; font-weight:bold; color:#ff4757; margin-top:5px;">💡必ずSNSも設定しておこう！</p>
                </div>
            </div>
        </div>

        <div class="button-group">
            <button id="copyBtn" class="copy-btn">
                <span class="os-label">Androidの方</span>
                📋 コピーしてアプリへ
            </button>
            <button id="openMixchannelBtn" class="mixchannel-btn">
                <span class="os-label">iPhoneの方</span>
                📱 コピーしてアプリへ
            </button>
        </div>
        <button id="resetBtn" class="reset-btn">🔄 全てリセット</button>
    </div>
</div>

<div id="toast" class="toast"></div>

<script>
    const phrases = [
        "笑顔と元気を届けるフルパワー配信！🔥", "みんなの日常を少しだけ明るくしたい🌸", "夢に向かって全力走中！",
        "癒やしの声であなたの夜を彩ります🌙", "雑談メインのまったりルームへようこそおこしやす🍵",
        "ギャップ萌え注意？見た目と中身は違います！😎", "あなたの推しになりたい！見つけてくれてありがとう💎",
        "歌うことと食べることが大好き！食いしん坊配信者🍚", "目指せ、ミクチャのトップランカー🌟",
        "毎日配信でみんなと繋がれる場所を作りたい🌱", "ゆるふわに見えて、実は負けず嫌いですっ！💪",
        "音楽で心を通わせたい。練習中のギターも聴いてね🎸", "誰よりも濃い時間を一緒に過ごしましょう！💖",
        "等身大の私を好きになってくれますか？✨", "元気がない日は私のところへおいで！ニコニコお届け🌈",
        "一度ハマったら抜け出せない？沼配信へようこそ😈", "将来の夢は日本一のモデル！一歩ずつ進んでます🦋",
        "人見知りだけど配信ではお喋り！仲良くしてね💕", "あなたの一番の理解者になりたいです🌷",
        "夢への第一歩、ここで踏み出します。応援してください！✨", "目指すはグランプリのみ。私と一緒に頂上を見ませんか？🏆",
        "本気だからこそ、全力で走り抜けます。後悔はさせません！🔥", "人生を変える1ヶ月。あなたの1ポチが私の力になります💪",
        "自分史上、最高の自分へ。最後まで食らいつきます！🏅", "不器用なりに全力投球。私の成長を見届けてください！🌟",
        "誰かの心に寄り添える、そんな存在になりたいです🕊️", "背伸びせず、私らしく。笑顔の花を咲かせます。🌸",
        "あなたの日常に、少しの彩りと癒しを。🍵", "一期一会を大切に。素敵な出会いに感謝して配信中💎",
        "等身大の大学生（高校生）。夢に向かって真っ直ぐ進みます☁️", "清楚×笑顔で、みんなの『一番』になりたいな🎀",
        "見た目はクール、中身は食いしん坊！？ギャップ萌え注意⚠️", "喋りだすと止まらない！ミスコン界の元気印です🌻",
        "唯一無二の存在感。あなたの推し枠に空きはありませんか？👀", "アニメとチョコが動力源。親しみやすさNo.1宣言！🍫",
        "クールに見えて、実はゲラです。笑いの絶えない枠へようこそ！😆", "偏差値より、みんなとの団結力を上げたい！📚✨",
        "夢は大きく、態度は謙虚に。応援お願いします！🌈", "私を見つけてくれてありがとう。運命にしちゃいませんか？💌",
        "掴み取りたい未来がある。全力走中！🏃‍♀️💨", "みんなの応援が、私の輝く魔法になります🪄",
        "1回きりの夏（冬）、最高の思い出を一緒に作ろう☀️", "今日も1日お疲れ様。あなたの安らぎの場所になりたい🌙",
        "私をグランプリに連れて行ってください！最高の景色を見せます🤝", "一人じゃ届かない場所も、みんなとなら行ける気がする🚀",
        "あなたの1分1秒を、私に投資してくれませんか？⏳✨", "目指せ伝説の枠！リスナーさんは全員、私の宝物です💎",
        "努力は裏切らない。それをこのイベントで証明したい📖", "今の私は未完成。みんなの応援で完成させてください！🎨"
    ];

    const eventSchedules = {
        "月刊わんこ掲載モデルオーディション": "……………………………………………………\n【月刊わんこ掲載モデルオーディション🐾】\n\nスタダ：2/23(月)~3/15(日)\n予選：3/27(金)~4/5(日)\n決勝：4/9(木)~4/22(水)\n……………………………………………………"
    };

    const fields = ['name', 'furigana', 'catchphrase', 'currentEvent', 'eventGoal', 'streamSchedule', 'content', 'awards', 'fanMark', 'dream', 'message'];

    document.addEventListener('DOMContentLoaded', () => {
        const phraseBtn = document.getElementById('randomPhraseBtn');
        const phraseTextarea = document.getElementById('catchphrase');

        phraseBtn.addEventListener('click', () => {
            phraseTextarea.value = phrases[Math.floor(Math.random() * phrases.length)];
            updateLivePreview();
        });

        document.querySelectorAll('input, textarea, select').forEach(el => {
            el.addEventListener('input', updateLivePreview);
        });

        document.getElementById('copyBtn').addEventListener('click', () => handleCopy("mixch://e/mypage/edit"));
        document.getElementById('openMixchannelBtn').addEventListener('click', () => handleCopy("mixch://mypage/edit"));
        document.getElementById('resetBtn').addEventListener('click', resetForm);

        loadDraft();
        updateLivePreview();
    });

    function generateProfile(data) {
        let p = `${data.name}${data.furigana ? '(' + data.furigana + ')' : ''} です！✨\n\n`;
        if (data.catchphrase) p += `${data.catchphrase}\n\n`;
        if (data.currentEvent) {
            p += (eventSchedules[data.currentEvent] || `……………………………………………………\n【${data.currentEvent} 参加中！】\n……………………………………………………`) + "\n\n";
        }
        if (data.eventGoal) p += `【目標】\n${data.eventGoal}\n\n`;
        if (data.streamSchedule) p += `【配信時間】\n${data.streamSchedule}\n\n`;
        if (data.content) p += `【内容】\n${data.content}\n\n`;
        if (data.awards) p += `🏆 受賞歴：\n${data.awards}\n\n`;
        if (data.fanMark) p += `ファンマーク：${data.fanMark}\n\n`;
        if (data.dream) p += `🌟 夢・目標\n${data.dream}\n\n`;
        if (data.message) p += `┈┈┈┈┈┈┈┈┈┈┈┈\n💌 メッセージ\n${data.message}\n`;
        return p;
    }

    function updateLivePreview() {
        const data = {};
        fields.forEach(f => data[f] = document.getElementById(f).value);
        const output = document.getElementById('profileOutput');
        
        if (!data.name) {
            output.textContent = 'お名前を入力すると自動生成されます';
        } else {
            output.textContent = generateProfile(data);
        }
        localStorage.setItem('mix_draft_pro_v2', JSON.stringify(data));
    }

    function handleCopy(url) {
        const text = document.getElementById('profileOutput').textContent;
        if (!text || text.includes('お名前を入力')) {
            alert('名前を入力してください');
            return;
        }
        navigator.clipboard.writeText(text).then(() => {
            showToast('📋 コピーしました！');
            setTimeout(() => { window.location.href = url; }, 800);
        });
    }

    function showToast(msg) {
        const t = document.getElementById('toast');
        t.textContent = msg;
        t.classList.add('show');
        setTimeout(() => t.classList.remove('show'), 2000);
    }

    function loadDraft() {
        const draft = JSON.parse(localStorage.getItem('mix_draft_pro_v2'));
        if (draft) {
            fields.forEach(key => {
                if (draft[key]) document.getElementById(key).value = draft[key];
            });
        }
    }

    function resetForm() {
        if (confirm('入力をすべて消去しますか？')) {
            document.getElementById('profileForm').reset();
            localStorage.removeItem('mix_draft_pro_v2');
            updateLivePreview();
        }
    }
</script>
</body>
</html>
