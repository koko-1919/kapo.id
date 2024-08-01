<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>無題ドキュメント</title>
</head>

<body>

    
    <!-- コピー対象要素とコピーボタン -->
    <input id="copyTarget" type="text" value="g39prh8f" readonly>
    <button onclick="copyToClipboard()">コピーする</button>


    <!-- bodyタグ内の下部に以下を入力する -->
    <script>
        function copyToClipboard() {
            // コピー対象をJavaScript上で変数として定義する
            var copyTarget = document.getElementById("copyTarget");

            // コピー対象のテキストを選択する
            copyTarget.select();

            // 選択しているテキストをクリップボードにコピーする
            document.execCommand("Copy");

            // コピーをお知らせする
            alert("フレンドコードをコピーしました : " + copyTarget.value);
        }
    </script>
</body>
</html>
