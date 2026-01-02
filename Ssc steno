<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Study Smart - SSC Steno Marks Calculator</title>
    <style>
        body { font-family: Arial, sans-serif; max-width: 800px; margin: 0 auto; padding: 20px; background: linear-gradient(135deg, #90EE90, #FFFF99); }
        .container { background: white; padding: 30px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
        h1 { color: #228B22; text-align: center; }
        label { display: block; margin: 10px 0 5px; font-weight: bold; }
        input, select { width: 100%; padding: 12px; margin-bottom: 15px; border: 1px solid #ddd; border-radius: 5px; box-sizing: border-box; font-size: 16px; }
        button { background: #007cba; color: white; padding: 15px 30px; border: none; border-radius: 5px; cursor: pointer; font-size: 18px; width: 100%; font-weight: bold; }
        button:hover { background: #005a87; }
        #result { margin-top: 20px; padding: 25px; background: #98FB98; border-radius: 5px; font-size: 20px; font-weight: bold; text-align: center; border: 2px solid #228B22; }
        .section { background: #f9f9f9; padding: 20px; border-radius: 5px; margin-bottom: 20px; }
    </style>
</head>
<body>
    <div class="container">
        <h1>SSC Stenographer Tier 1 Marks Calculator - Study Smart</h1>
        <p style="text-align: center; color: #666;">Apne correct aur wrong answers daalein, score calculate karein! (Total 200 Qs)</p>
        
        <div class="section">
            <label for="correct">Correct Answers (सही उत्तर):</label>
            <input type="number" id="correct" min="0" max="200" value="0">
            
            <label for="wrong">Wrong Answers (गलत उत्तर):</label>
            <input type="number" id="wrong" min="0" max="200" value="0">
        </div>
        
        <button onclick="calculateScore()">Calculate Marks (स्कोर निकालें)</button>
        
        <div id="result"></div>
        
        <div style="margin-top: 30px; font-size: 14px; color: #666; text-align: center;">
            Marking: +1 correct, -0.25 wrong | Unattempted: 0 <br>
            Study Smart - Free Exam Tools
        </div>
    </div>
    
    <script>
        function calculateScore() {
            const correct = parseInt(document.getElementById('correct').value) || 0;
            const wrong = parseInt(document.getElementById('wrong').value) || 0;
            const attempted = correct + wrong;
            if (attempted > 200 || correct < 0 || wrong < 0) {
                document.getElementById('result').innerHTML = 'Invalid input! Total attempts <= 200.';
                return;
            }
            const score = correct * 1 - wrong * 0.25;
            const unattempted = 200 - attempted;
            document.getElementById('result').innerHTML = `
                Your Score: <span style="color: #228B22; font-size: 28px;">${score.toFixed(2)}</span> / 200 <br>
                Correct: ${correct} (+${correct}) <br>
                Wrong: ${wrong} (-${(wrong*0.25).toFixed(2)}) <br>
                Unattempted: ${unattempted} (0)
            `;
        }
    </script>
</body>
</html>
