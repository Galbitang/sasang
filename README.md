<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QSCC II+ 사상체질분류 검사</title>
    <style>
        body { font-family: sans-serif; line-height: 1.6; }
        .question-group { margin-bottom: 20px; padding: 10px; border: 1px solid #eee; border-radius: 5px; }
        .question-text { font-weight: bold; margin-bottom: 8px; }
        label { display: block; margin-bottom: 5px; cursor: pointer; }
        input[type="radio"], input[type="checkbox"] { margin-right: 5px; }
        .instructions { background-color: #f0f8ff; padding: 15px; margin-bottom: 20px; border-radius: 5px; border: 1px solid #add8e6; }
        h1, h2 { border-bottom: 1px solid #ccc; padding-bottom: 5px; margin-top: 30px; }
        button { padding: 10px 15px; font-size: 1em; cursor: pointer; background-color: #007bff; color: white; border: none; border-radius: 5px; margin-top: 20px;}
        button:hover { background-color: #0056b3; }
        #result { margin-top: 20px; padding: 15px; border: 1px solid #ccc; background-color: #f9f9f9; border-radius: 5px; }
        #result h3 { margin-top: 0; }
        .error { color: red; font-weight: bold; }
    </style>
</head>
<body>

    <h1>QSCC II+ 사상체질분류 검사</h1>

    <div class="instructions">
        <p>본 검사지는 덕양구보건소에서 귀하의 체질을 감별할 목적으로 제공되었습니다.</p>
        <p>모든 로직은 사상체질분류검사지Ⅱ(QSCCⅡ)의 연구에 기반하여 만들어졌습니다.</p>
        <p><strong>설문에 답하는 요령</strong></p>
        <ol>
            <li>다음 설문 문항을 주의깊게 읽은 다음, 자신에게 가장 가깝다고 생각되는 내용을 선택하십시오.</li>
            <li>A형 문항(1-12번)은 가장 가까운 것 1개만 선택하고, B형 문항(13-54번)은 해당하는 모든 항목을 선택하십시오.</li>
            <li>자연스러운 마음가짐으로 응답해주십시오.</li>
        </ol>
        <p><strong>주의사항</strong> </p>
        <ol>
            <li>이 결과는 제공된 연구(강민수, 2019년도 경희대학교 석사논문)를 기반으로 한 예시입니다.</li>
            <li>정밀한 체질 진단을 위해서는 가까운 한의원에 내방하시길 바랍니다.</li>
        </ol>
    </div>

    <form id="qsccForm">
        <h2>A형 문항 (가장 가까운 것 1개 선택)</h2>

        <div class="question-group">
            <p class="question-text">1. 당신의 체격은 어떻습니까?</p>
            <label><input type="radio" name="q1" value="1"> ① 체격이 큰 편이다.</label>
            <label><input type="radio" name="q1" value="2"> ② 보통이다.</label>
            <label><input type="radio" name="q1" value="3"> ③ 체격이 작은 편이다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">2. 당신의 체형은 어떻습니까?</p>
            <label><input type="radio" name="q2" value="1"> ① 뚱뚱한 편이다.</label>
            <label><input type="radio" name="q2" value="2"> ② 보통이다.</label>
            <label><input type="radio" name="q2" value="3"> ③ 마른 편이다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">3. 당신의 체형에서 상하체의 관계는 어떻습니까?</p>
            <label><input type="radio" name="q3" value="1"> ① 상체가 하체에 비하여 발달되어 있다.</label>
            <label><input type="radio" name="q3" value="2"> ② 하체가 상체에 비하여 발달되어 있다.</label>
            <label><input type="radio" name="q3" value="3"> ③ 상하체가 비슷하다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">4. 다음중 당신의 체형은 어디에 해당됩니까?</p>
            <label><input type="radio" name="q4" value="1"> ① 목덜미부위가 잘 발달하고 허리부위가 빈약하다.</label>
            <label><input type="radio" name="q4" value="2"> ② 가슴부위가 잘 발달하고 엉덩이부위가 빈약하다.</label>
            <label><input type="radio" name="q4" value="3"> ③ 허리부위가 잘 발달하고 목덜미부위가 빈약하다.</label>
            <label><input type="radio" name="q4" value="4"> ④ 엉덩이부위가 잘 발달하였고 가슴부위가 빈약하다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">5. 전체적인 외모와 골격은 다음중 어디에 해당됩니까?</p>
            <label><input type="radio" name="q5" value="1"> ① 골격이 굵고 살이 찐 편이다.</label>
            <label><input type="radio" name="q5" value="2"> ② 골격이 작고 균형이 잡혀있다.</label>
            <label><input type="radio" name="q5" value="3"> ③ 보통이며 다부진 체격이다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">6. 당신의 가슴은 다음중 어디에 해당됩니까?</p>
            <label><input type="radio" name="q6" value="1"> ① 넓고 잘 발달되어 있다. (비만형)</label>
            <label><input type="radio" name="q6" value="2"> ② 빈약하고 구부정하다. (세장형)</label>
            <label><input type="radio" name="q6" value="3"> ③ 넓고 튼튼한 편이다. (근육형)</label>
            <label><input type="radio" name="q6" value="4"> ④ 가슴이 벌어지고 견실하다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">7. 당신은 다음중 어떤 음식을 좋아하십니까?</p>
            <label><input type="radio" name="q7" value="1"> ① 뜨거운 음식</label>
            <label><input type="radio" name="q7" value="2"> ② 따뜻한 음식</label>
            <label><input type="radio" name="q7" value="3"> ③ 시원한 음식</label>
            <label><input type="radio" name="q7" value="4"> ④ 차가운 음식</label>
        </div>

        <div class="question-group">
            <p class="question-text">8. 당신은 다음중 어디에 해당됩니까?</p>
            <label><input type="radio" name="q8" value="1"> ① 평소 손, 발이 찬 편이다.</label>
            <label><input type="radio" name="q8" value="2"> ② 평소 손, 발이 따뜻한 편이다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">9. 당신의 걸음걸이는 다음중 어디에 해당됩니까?</p>
            <label><input type="radio" name="q9" value="1"> ① 걸음이 느리고 무게 있게 걷는다.</label>
            <label><input type="radio" name="q9" value="2"> ② 걸음걸이가 자연스럽고 얌전하다.</label>
            <label><input type="radio" name="q9" value="3"> ③ 걸음이 빠르고 몸을 흔든다.</label>
            <label><input type="radio" name="q9" value="4"> ④ 걸음걸이가 꼿꼿하다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">10. 당신은 다음중 어디에 해당됩니까?</p>
            <label><input type="radio" name="q10" value="1"> ① 평소에 땀이 많고 땀을 흘리면 오히려 상쾌하다.</label>
            <label><input type="radio" name="q10" value="2"> ② 평소에 땀이 많지 않고 조금만 땀을 내도 피곤하다.</label>
            <label><input type="radio" name="q10" value="3"> ③ 땀을 흘려도 그다지 피곤하지 않다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">11. 당신은 다음중 어디에 해당됩니까?</p>
            <label><input type="radio" name="q11" value="1"> ① 거침없고 과단성이 있다.</label>
            <label><input type="radio" name="q11" value="2"> ② 활동적이고 용감하다.</label>
            <label><input type="radio" name="q11" value="3"> ③ 용모가 의젓하고 격식을 차리는 편이다.</label>
            <label><input type="radio" name="q11" value="4"> ④ 태도가 온순하고 꾸밈이 없다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">12. 다음중 당신은 어느 쪽입니까? (일처리, 또는 생활습관)</p>
            <label><input type="radio" name="q12" value="1"> ① 무슨 일이든지 물러서지 않고 밀고 나간다.</label>
            <label><input type="radio" name="q12" value="2"> ② 일을 벌려 놓기만 하지 마무리를 잘 하지 못한다.</label>
            <label><input type="radio" name="q12" value="3"> ③ 움직이기보다는 조용히 혼자 일을 추진하는 편이다.</label>
            <label><input type="radio" name="q12" value="4"> ④ 한곳에 있으려고만하지 나다니려하지 않는 편이다.</label>
        </div>

        <h2>B형 문항 (일치하는 문항 모두 선택)</h2>
        <p>아래의 설문 문항들을 주의 깊게 읽은 다음, 자신이 일상적인 느낌이나 행동과 일치한다고 생각되는 문항에 모두 선택하여 주십시오.</p>

        <div class="question-group">
            <p class="question-text">13. 일처리와 장단점 (모두 고르기) </p>
            <label><input type="checkbox" name="q13" value="1"> 무슨 일이나 시원스럽게 처리한다.</label>
            <label><input type="checkbox" name="q14" value="1"> 활발하고 대가 센 편이다.</label>
            <label><input type="checkbox" name="q15" value="1"> 매사에 이해를 따지지 않고 나서는 편이다.</label>
            <label><input type="checkbox" name="q16" value="1"> 진득하게 한곳에 오래 앉을 수 있다.</label>
            <label><input type="checkbox" name="q17" value="1"> 치밀하고 꼼꼼한 편이다.</label>
            <label><input type="checkbox" name="q18" value="1"> 가까운 사람끼리만 어울리는 편이다.</label>
            <label><input type="checkbox" name="q19" value="1"> 사람을 사귈 때 이것저것 따지지 않고 쉽게 잘 사귄다.</label>
            <label><input type="checkbox" name="q20" value="1"> 사회적인 일보다 개인적인 일에 열심이다.</label>
            <label><input type="checkbox" name="q21" value="1"> 내면적인 것보다 외면적인 것을 더 중요시한다.</label>
            <label><input type="checkbox" name="q22" value="1"> 사람을 사귈 때 이것저것 따져서 쉽게 사귀지 못하는 편이다.</label>
            <label><input type="checkbox" name="q23" value="1"> 단정하고 신중하다.</label>
            <label><input type="checkbox" name="q24" value="1"> 성격이 시원시원하다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">14. 대인관계 (모두 고르기) </p>
            <label><input type="checkbox" name="q25" value="1"> 다정 다감하여 남을 잘 달랜다.</label>
            <label><input type="checkbox" name="q26" value="1"> 각종 사회활동 모임에 즐거이 참여한다.</label>
            <label><input type="checkbox" name="q27" value="1"> 나는 사람을 볼 때 그 사람이 부지런한지 아닌지를 금방 알아차린다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">15. 평소의 마음 (모두 고르기) </p>
            <label><input type="checkbox" name="q28" value="1"> 항상 급하게 서두르는 편이다.</label>
            <label><input type="checkbox" name="q29" value="1"> 처음에 남앞에 잘 나서지 못한다.</label>
            <label><input type="checkbox" name="q30" value="1"> 평소 소심하여 항상 불안한 편이다.</label>
            <label><input type="checkbox" name="q31" value="1"> 평소에 신경이 예민한 편이다.</label>
            <label><input type="checkbox" name="q32" value="1"> 인내심이 많다.</label>
            <label><input type="checkbox" name="q33" value="1"> 행동이 경솔한 편이다.</label>
            <label><input type="checkbox" name="q34" value="1"> 별일이 아닌데도 조바심치며 불안해한다.</label>
            <label><input type="checkbox" name="q35" value="1"> 남성적인 면이 많고 여성적인 면이 적다.</label>
        </div>

        <div class="question-group">
             <p class="question-text">16. 문제점 (모두 고르기)</p>
            <label><input type="checkbox" name="q36" value="1"> 별것 아닌 사소한 일 때문에 짜증을 내곤 한다.</label>
            <label><input type="checkbox" name="q37" value="1"> 앞에 나가서 말을 하거나 발표하는 것이 어렵다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">17. 감정 특성 (모두 고르기)</p>
            <label><input type="checkbox" name="q38" value="1"> 평소에는 명랑하지만 감정의 기복이 심한 편이다.</label>
            <label><input type="checkbox" name="q39" value="1"> 마음이 상했더라도 괜찮은 척 한다.</label>
            <label><input type="checkbox" name="q40" value="1"> 업신여김을 당하면 화가 나서 주체할 수 없다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">18. 행동 특성 (모두 고르기)</p>
            <label><input type="checkbox" name="q41" value="1"> 내 생각이 옳다고 확신되기까지는 함부로 말하지 않는다.</label>
            <label><input type="checkbox" name="q42" value="1"> 아는 척 하거나 과시하는 경우가 많다.</label>
            <label><input type="checkbox" name="q43" value="1"> 자신에게는 소홀히하고 남에게는 깍듯이 대한다.</label>
            <label><input type="checkbox" name="q44" value="1"> 남앞에 잘 나서지 못한다.</label>
            <label><input type="checkbox" name="q45" value="1"> 남을 의식하지 않고 내 멋대로 하는 편이다.</label>
            <label><input type="checkbox" name="q46" value="1"> 소심하여 항상 불안한 편이다.</label>
            <label><input type="checkbox" name="q47" value="1"> 여성적인 면이 많고 남성적인 면이 적다.</label>
            <label><input type="checkbox" name="q48" value="1"> 웬만한 일을 성취하였어도 부족함을 느낄 때가 많다.</label>
        </div>

        <div class="question-group">
            <p class="question-text">19. 몸상태 (모두 고르기)</p>
            <label><input type="checkbox" name="q49" value="1"> 이유없이 토하거나 음식을 삼키기가 어려운 적이 있었다.</label>
            <label><input type="checkbox" name="q50" value="1"> 몸이 안 좋을 때 땀을 내면 개운하다.</label>
            <label><input type="checkbox" name="q51" value="1"> 몸이 안 좋으면 소화가 잘 되지 않는다.</label>
            <label><input type="checkbox" name="q52" value="1"> 평소에 기운이 없어 한숨을 내쉬는 경우가 자주 있다.</label>
            <label><input type="checkbox" name="q53" value="1"> 온몸과 다리가 힘이 빠져 움직이기가 어려운 증상을 경험한 적이 있다.</label>
            <label><input type="checkbox" name="q54" value="1"> 음식을 먹은 후 가슴과 배가 더부룩한 증상이 자주 있다.</label>
        </div>

        <button type="button" onclick="calculateResult()">결과 확인</button>

    </form>

    <div id="result"></div>

    <script>
        function calculateResult() {
            const form = document.getElementById('qsccForm');
            const resultDiv = document.getElementById('result');
            resultDiv.innerHTML = ''; // 이전 결과 지우기

            let sePoints = 0; // 소음인 (SE)
            let syPoints = 0; // 소양인 (SY)
            let tePoints = 0; // 태음인 (TE)
            let unanswered = [];

            // A형 문항 (1-12번) 점수 계산
            for (let i = 1; i <= 12; i++) {
                const qName = 'q' + i;
                const selectedRadio = form.elements[qName];
                if (!selectedRadio || !selectedRadio.value) {
                    unanswered.push(`A형 ${i}번`);
                    continue;
                }
                const choice = selectedRadio.value;

                switch (qName) {
                    case 'q1': // 체격
                        if (choice === '1') tePoints += 1; // 체격이 큰 편이다.
                        if (choice === '3') sePoints += 1; // 체격이 작은 편이다.
                        break;
                    case 'q2': // 체형
                        if (choice === '1') tePoints += 1; // 뚱뚱한 편이다.
                        if (choice === '3') sePoints += 1; // 마른 편이다.
                        break;
                    case 'q3': // 상하체 관계
                        if (choice === '1') syPoints += 1; // 상체가 하체에 비하여 발달되어 있다.
                        if (choice === '2') tePoints += 1; // 하체가 상체에 비하여 발달되어 있다.
                        if (choice === '3') sePoints += 1; // 상하체가 비슷하다.
                        break;
                    case 'q4': // 체형 (세부)
                        if (choice === '1') syPoints += 1; // 목덜미 발달, 허리 빈약
                        if (choice === '2') sePoints += 1; // 가슴 발달, 엉덩이 빈약
                        if (choice === '3') tePoints += 1; // 허리 발달, 목덜미 빈약
                        if (choice === '4') sePoints += 1; // 엉덩이 발달, 가슴 빈약
                        break;
                    case 'q5': // 외모, 골격
                        if (choice === '1') tePoints += 1; // 골격이 굵고 살이 찐 편이다.
                        if (choice === '2') sePoints += 1; // 골격이 작고 균형이 잡혀있다.
                        if (choice === '3') syPoints += 1; // 보통이며 다부진 체격이다.
                        break;
                    case 'q6': // 가슴
                        if (choice === '1') tePoints += 1; // 넓고 잘 발달되어 있다. (비만형)
                        if (choice === '2') sePoints += 1; // 빈약하고 구부정하다. (세장형)
                        if (choice === '3') syPoints += 1; // 넓고 튼튼한 편이다. (근육형)
                        if (choice === '4') syPoints += 1; // 가슴이 벌어지고 견실하다. (이 경우, 강민수 논문 Table 9에 명확한 점수 없음. SY로 임시 할당.)
                        break;
                    case 'q7': // 좋아하는 음식
                        if (choice === '3') syPoints += 1; // 시원한 음식 (강민수 논문 Table 9에 SY 1점 배정)
                        // Q7은 다른 선택지에 대한 점수가 논문에 명시되어 있지 않음.
                        break;
                    case 'q8': // 손, 발 온도
                        if (choice === '1') sePoints += 1; // 손, 발이 찬 편이다.
                        if (choice === '2') syPoints += 1; // 손, 발이 따뜻한 편이다.
                        break;
                    case 'q9': // 걸음걸이
                        if (choice === '1') tePoints += 1; // 걸음이 느리고 무게 있게 걷는다.
                        if (choice === '2') sePoints += 1; // 걸음걸이가 자연스럽고 얌전하다.
                        if (choice === '3') syPoints += 1; // 걸음이 빠르고 몸을 흔든다.
                        if (choice === '4') syPoints += 1; // 걸음걸이가 꼿꼿하다. (강민수 논문 Table 9에 SY 1점 배정)
                        break;
                    case 'q10': // 땀
                        if (choice === '1') tePoints += 1; // 땀이 많고 흘리면 상쾌
                        if (choice === '2') sePoints += 1; // 땀이 많지 않고 흘리면 피곤
                        // Q10-3은 논문에 명시된 점수 없음.
                        break;
                    case 'q11': // 성격 (과단성, 활동적, 의젓, 온순)
                        if (choice === '1') syPoints += 1; // 거침없고 과단성이 있다.
                        if (choice === '2') syPoints += 1; // 활동적이고 용감하다.
                        if (choice === '3') tePoints += 1; // 용모가 의젓하고 격식을 차리는 편이다.
                        if (choice === '4') sePoints += 1; // 태도가 온순하고 꾸밈이 없다.
                        break;
                    case 'q12': // 일처리, 생활습관
                        if (choice === '1') syPoints += 1; // 물러서지 않고 밀고 나간다.
                        if (choice === '2') syPoints += 1; // 일을 벌려 놓기만 하지 마무리를 잘 하지 못한다.
                        if (choice === '3') sePoints += 1; // 조용히 혼자 일을 추진하는 편이다.
                        if (choice === '4') tePoints += 1; // 한곳에 있으려만 하고 나다니려 하지 않는다.
                        break;
                }
            }

            // B형 문항 (13-54번) 점수 계산
            for (let i = 13; i <= 54; i++) {
                const qName = 'q' + i;
                const checkboxes = form.querySelectorAll(`input[name="${qName}"]:checked`);
                // B형 문항은 '모두 선택'이므로, 하나라도 선택되었는지 확인
                // 또한, Table 10에서 N(아니오)일 때 점수가 부여되는 문항들이 있으므로,
                // 선택되지 않았을 때의 점수도 고려해야 함.
                // 편의상, 여기에선 단순히 '선택했을 때'만 점수를 부여하도록 논문을 따름.
                // 논문에 N일 때 점수가 있는 항목은 체크되지 않았을 때 점수 부여 (예: q13)

                const isChecked = checkboxes.length > 0;

                switch (qName) {
                    case 'q13': if (!isChecked) sePoints += 1; break; // 시원스럽게 처리한다. (N일 때 SE +1)
                    case 'q14': if (!isChecked) sePoints += 1; break; // 활발하고 대가 센 편이다. (N일 때 SE +1)
                    case 'q15': if (isChecked) syPoints += 1; break; // 매사에 이해를 따지지 않고 나서는 편이다. (Y일 때 SY +1)
                    case 'q16': if (isChecked) { sePoints += 1; tePoints += 1; } break; // 진득하게 한곳에 오래 앉을 수 있다. (Y일 때 SE +1, TE +1)
                    case 'q17': if (!isChecked) { syPoints += 1; tePoints += 1; } break; // 치밀하고 꼼꼼한 편이다. (N일 때 SY +1, TE +1)
                    case 'q18': if (isChecked) sePoints += 1; break; // 가까운 사람끼리만 어울리는 편이다. (Y일 때 SE +1)
                    case 'q19': if (!isChecked) sePoints += 1; break; // 사람을 사귈 때 이것저것 따지지 않고 쉽게 잘 사귄다. (N일 때 SE +1)
                    case 'q20': if (isChecked) sePoints += 1; break; // 사회적인 일보다 개인적인 일에 열심이다. (Y일 때 SE +1)
                    case 'q21': if (isChecked) syPoints += 1; break; // 내면적인 것보다 외면적인 것을 더 중요시한다. (Y일 때 SY +1)
                    case 'q22': if (isChecked) tePoints += 1; break; // 사람을 사귈 때 이것저것 따져서 쉽게 사귀지 못하는 편이다. (Y일 때 TE +1)
                    case 'q23': if (isChecked) tePoints += 1; break; // 단정하고 신중하다. (Y일 때 TE +1)
                    case 'q24': if (!isChecked) sePoints += 1; break; // 성격이 시원시원하다. (N일 때 SE +1)
                    case 'q25': if (isChecked) sePoints += 1; break; // 다정 다감하여 남을 잘 달랜다. (Y일 때 SE +1)
                    case 'q26': if (!isChecked) sePoints += 1; break; // 각종 사회활동 모임에 즐거이 참여한다. (N일 때 SE +1)
                    case 'q27': if (isChecked) { syPoints += 1; tePoints += 1; } break; // 나는 사람을 볼 때 그 사람이 부지런한지 아닌지를 금방 알아차린다. (Y일 때 SY +1, TE +1)
                    case 'q28': if (isChecked) syPoints += 1; break; // 항상 급하게 서두르는 편이다. (Y일 때 SY +1)
                    case 'q29': if (isChecked) sePoints += 1; break; // 처음에 남앞에 잘 나서지 못한다. (Y일 때 SE +1)
                    case 'q30': if (isChecked) sePoints += 1; break; // 평소 소심하여 항상 불안한 편이다. (Y일 때 SE +1)
                    case 'q31': if (isChecked) sePoints += 1; break; // 평소에 신경이 예민한 편이다. (Y일 때 SE +1)
                    case 'q32': if (isChecked) tePoints += 1; break; // 인내심이 많다. (Y일 때 TE +1)
                    case 'q33': if (isChecked) syPoints += 1; break; // 행동이 경솔한 편이다. (Y일 때 SY +1)
                    case 'q34': if (isChecked) sePoints += 1; break; // 별일이 아닌데도 조바심치며 불안해한다. (Y일 때 SE +1)
                    case 'q35': if (!isChecked) { sePoints += 1; tePoints += 1; } break; // 남성적인 면이 많고 여성적인 면이 적다. (N일 때 SE +1, TE +1)
                    case 'q36': if (isChecked) syPoints += 1; break; // 별것 아닌 사소한 일 때문에 짜증을 내곤 한다. (Y일 때 SY +1)
                    case 'q37': if (isChecked) sePoints += 1; break; // 앞에 나가서 말을 하거나 발표하는 것이 어렵다. (Y일 때 SE +1)
                    case 'q38': if (isChecked) syPoints += 1; break; // 평소에는 명랑하지만 감정의 기복이 심한 편이다. (Y일 때 SY +1)
                    case 'q39': if (isChecked) tePoints += 1; break; // 마음이 상했더라도 괜찮은 척 한다. (Y일 때 TE +1)
                    case 'q40': if (isChecked) syPoints += 1; break; // 업신여김을 당하면 화가 나서 주체할 수 없다. (Y일 때 SY +1)
                    case 'q41': if (isChecked) tePoints += 1; break; // 내 생각이 옳다고 확신되기까지는 함부로 말하지 않는다. (Y일 때 TE +1)
                    case 'q42': if (isChecked) syPoints += 1; break; // 아는 척 하거나 과시하는 경우가 많다. (Y일 때 SY +1)
                    case 'q43': if (isChecked) tePoints += 1; break; // 자신에게는 소홀히하고 남에게는 깍듯이 대한다. (Y일 때 TE +1)
                    case 'q44': if (!isChecked) syPoints += 1; break; // 남앞에 잘 나서지 못한다. (N일 때 SY +1)
                    case 'q45': if (isChecked) syPoints += 1; break; // 남을 의식하지 않고 내 멋대로 하는 편이다. (Y일 때 SY +1)
                    case 'q46': if (isChecked) sePoints += 1; break; // 소심하여 항상 불안한 편이다. (Y일 때 SE +1)
                    case 'q47': if (isChecked) { sePoints += 1; syPoints += 1; } break; // 여성적인 면이 많고 남성적인 면이 적다. (Y일 때 SE +1, SY +1)
                    case 'q48': if (isChecked) tePoints += 1; break; // 웬만한 일을 성취하였어도 부족함을 느낄 때가 많다. (Y일 때 TE +1)
                    case 'q49': if (isChecked) syPoints += 1; break; // 이유없이 토하거나 음식을 삼키기가 어려운 적이 있었다. (Y일 때 SY +1)
                    case 'q50': if (isChecked) tePoints += 1; break; // 몸이 안 좋을 때 땀을 내면 개운하다. (Y일 때 TE +1)
                    case 'q51': if (isChecked) { sePoints += 1; syPoints += 1; } break; // 몸이 안 좋으면 소화가 잘 되지 않는다. (Y일 때 SE +1, SY +1)
                    case 'q52': if (isChecked) sePoints += 1; break; // 평소에 기운이 없어 한숨을 내쉬는 경우가 자주 있다. (Y일 때 SE +1)
                    case 'q53': if (isChecked) tePoints += 1; break; // 온몸과 다리가 힘이 빠져 움직이기가 어려운 증상을 경험한 적이 있다. (Y일 때 TE +1)
                    case 'q54': if (isChecked) tePoints += 1; break; // 음식을 먹은 후 가슴과 배가 더부룩한 증상이 자주 있다. (Y일 때 TE +1)
                }
            }

            if (unanswered.length > 0) {
                resultDiv.innerHTML = `<h3 class="error">모든 질문에 답해주세요!</h3><p class="error">답변하지 않은 문항: ${unanswered.join(', ')}</p>`;
                return;
            }

            // 결과 판별
            let maxPoints = Math.max(sePoints, syPoints, tePoints);
            let resultTrait = '';
            let traits = [];

            if (sePoints === maxPoints) traits.push('소음인');
            if (syPoints === maxPoints) traits.push('소양인');
            if (tePoints === maxPoints) traits.push('태음인');

            if (traits.length === 1) {
                resultTrait = traits[0];
            } else if (traits.length > 1) {
                resultTrait = '특정 체질로 판별하기 어려움 (복수 체질)';
                // 동점인 경우, 추가적인 판별 기준이 있다면 여기에 로직 추가 가능
                // 예를 들어, 소음인-소양인 동점 시 태양인 가능성 등
            } else {
                resultTrait = '판별할 수 없는 결과';
            }

            resultDiv.innerHTML = `
                <h3>체질 판별 결과</h3>
                <p><strong>소음인 점수:</strong> ${sePoints}점</p>
                <p><strong>소양인 점수:</strong> ${syPoints}점</p>
                <p><strong>태음인 점수:</strong> ${tePoints}점</p>
                <p><strong>당신의 체질은: <span style="color: blue; font-weight: bold;">${resultTrait}</span></strong> 입니다.</p>
                ${resultTrait === '특정 체질로 판별하기 어려움 (복수 체질)' ? '<p>동점인 체질: ' + traits.join(', ') + '</p>' : ''}
            `;
        }
    </script>

</body>
</html>
