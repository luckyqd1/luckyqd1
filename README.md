<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>生日快乐!</title>
    <style>
        @import url("https://fonts.googleapis.com/css?family=Concert+One|Pacifico");

        .mobile {
            position: fixed;
            text-align: center;
            width: 100%;
            top: 50px;
            font-size: 90px;
            display: block;
        }

        h1, h2, h3, span {
            display: none;
        }

        @media screen and (min-width: 670px) {
            .mobile {
                display: none;
            }

            h1, h2, h3, span {
                display: block;
            }

            body {
                background: linear-gradient(to right, #e2b8f7, #d4bafa, #c7bcfb, #b9befb, #acbff9);
                cursor: crosshair;
                perspective: 1000px;
                transform-style: preserve-3d;
                font-family: "Pacifico", cursive;
            }

            h1 {
                position: fixed;
                text-align: center;
                width: 100%;
                top: 120px;
                font-size: 90px;
                background: -webkit-linear-gradient(0deg, #ceadfc 0%, #a3bbfb 100%);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
                font-family: 'Concert One', cursive;
                font-weight: 400;
                z-index: -1;
                letter-spacing: 6px;
            }

            span {
                position: fixed;
                text-align: center;
                width: 100%;
                top: 70px;
                font-size: 70px;
            }

            h3 {
                position: fixed;
                text-align: center;
                width: 100%;
                top: 80px;
                font-size: 80px;
                background: -webkit-linear-gradient(90deg, #e9e6ff 0%, white 100%);
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;
            }

            bokeh {
                position: fixed;
                width: 2vmin;
                height: 2vmin;
                border-radius: 50%;
                animation-name: explosion;
                animation-iteration-count: infinite;
                animation-direction: reverse;
                animation-timing-function: cubic-bezier(0.84, 0.02, 1, 1);
            }

            bokeh:nth-child(1) {
                background-color: #2bd8ff;
                transform: translate(70.7404476506vw, 39.2982912115vh);
                animation-duration: 2.451477853s;
                animation-delay: -3.9090695973s;
            }

            bokeh:nth-child(2) {
                background-color: #feff28;
                transform: translate(21.390916309vw, 83.9320950239vh);
                animation-duration: 2.6082661613s;
                animation-delay: -2.4177632704s;
            }

            bokeh:nth-child(3) {
                background-color: #feff28;
                transform: translate(99.4707896083vw, 50.8779038063vh);
                animation-duration: 2.3934609219s;
                animation-delay: -4.9374235187s;
            }

            bokeh:nth-child(4) {
                background-color: #ef8d22;
                transform: translate(88.0762428158vw, 60.8758646268vh);
                animation-duration: 4.3745762554s;
                animation-delay: -4.2335574629s;
            }

            bokeh:nth-child(5) {
                background-color: #feff28;
                transform: translate(87.209776097vw, 87.4722435411vh);
                animation-duration: 2.6247180243s;
                animation-delay: -0.3571633852s;
            }

            bokeh:nth-child(6) {
                background-color: #feff28;
                transform: translate(67.5348277973vw, 93.8934516001vh);
                animation-duration: 3.0630744908s;
                animation-delay: -4.4890304964s;
            }

            bokeh:nth-child(7) {
                background-color: #feff28;
                transform: translate(51.2278043561vw, 39.0030857051vh);
                animation-duration: 3.1065374294s;
                animation-delay: -4.5619134997s;
            }

            bokeh:nth-child(8) {
                background-color: #fc85e1;
                transform: translate(63.2547804674vw, 88.7449965817vh);
                animation-duration: 2.8384921355s;
                animation-delay: -0.0965491775s;
            }

            bokeh:nth-child(9) {
                background-color: #fc85e1;
                transform: translate(1.7747115187vw, 78.6520215079vh);
                animation-duration: 4.3100039072s;
                animation-delay: -0.553894004s;
            }

            bokeh:nth-child(10) {
                background-color: #ef8d22;
                transform: translate(61.1915375825vw, 46.9592056036vh);
                animation-duration: 2.6244512022s;
                animation-delay: -4.5897035553s;
            }

            bokeh:nth-child(11) {
                background-color: #ef8d22;
                transform: translate(4.3118502657vw, 31.3689335931vh);
                animation-duration: 2.9020870937s;
                animation-delay: -0.0475365525s;
            }

            bokeh:nth-child(12) {
                background-color: #fc85e1;
                transform: translate(11.7124176675vw, 39.3853134156vh);
                animation-duration: 2.7165067308s;
                animation-delay: -0.3402677425s;
            }

            bokeh:nth-child(13) {
                background-color: #fc85e1;
                transform: translate(94.2835231134vw, 15.247368654vh);
                animation-duration: 3.1761028617s;
                animation-delay: -4.3999397039s;
            }

            bokeh:nth-child(14) {
                background-color: #ef8d22;
                transform: translate(22.7721270307vw, 68.9730094645vh);
                animation-duration: 3.6217481701s;
                animation-delay: -4.3121585024s;
            }

            bokeh:nth-child(15) {
                background-color: #2bd8ff;
                transform: translate(82.1182207545vw, 11.2392421851vh);
                animation-duration: 3.4960993434s;
                animation-delay: -3.7739573258s;
            }

            bokeh:nth-child(16) {
                background-color: #2bd8ff;
                transform: translate(19.7968006723vw, 77.2717558727vh);
                animation-duration: 3.1354637591s;
                animation-delay: -2.8370634184s;
            }

            bokeh:nth-child(17) {
                background-color: #feff28;
                transform: translate(84.4109063964vw, 23.5168492096vh);
                animation-duration: 4.3723964886s;
                animation-delay: -1.7390935649s;
            }

            bokeh:nth-child(18) {
                background-color: #fc85e1;
                transform: translate(72.7671083205vw, 62.5592027903vh);
                animation-duration: 4.4313534479s;
                animation-delay: -3.0082038529s;
            }

            bokeh:nth-child(19) {
                background-color: #2bd8ff;
                transform: translate(79.3141365436vw, 1.3143345978vh);
                animation-duration: 2.392781523s;
                animation-delay: -0.261672225s;
            }

            bokeh:nth-child(20) {
                background-color: #ef8d22;
                transform: translate(29.2041570725vw, 86.8219678576vh);
                animation-duration: 3.7180833613s;
                animation-delay: -1.7317238209s;
            }

            bokeh:nth-child(21) {
                background-color: #2bd8ff;
                transform: translate(72.3682688076vw, 29.3261143931vh);
                animation-duration: 3.5629502006s;
                animation-delay: -4.5261179684s;
            }

            bokeh:nth-child(22) {
                background-color: #2bd8ff;
                transform: translate(41.7909696011vw, 5.9456249418vh);
                animation-duration: 2.7586444687s;
                animation-delay: -1.2172526656s;
            }

            bokeh:nth-child(23) {
                background-color: #feff28;
                transform: translate(76.2571451639vw, 17.195474965vh);
                animation-duration: 4.4228449437s;
                animation-delay: -0.4973092974s;
            }

            bokeh:nth-child(24) {
                background-color: #2bd8ff;
                transform: translate(64.8267410528vw, 72.3685961754vh);
                animation-duration: 4.0308729373s;
                animation-delay: -3.4748753047s;
            }

            bokeh:nth-child(25) {
                background-color: #feff28;
                transform: translate(51.9640189709vw, 48.6043629666vh);
                animation-duration: 3.1974276784s;
                animation-delay: -1.6166953152s;
            }

            bokeh:nth-child(26) {
                background-color: #ef8d22;
                transform: translate(41.1498699458vw, 47.5398372353vh);
                animation-duration: 4.8552340393s;
                animation-delay: -0.9697552189s;
            }

            bokeh:nth-child(27) {
                background-color: #2bd8ff;
                transform: translate(81.3954514701vw, 46.9511786798vh);
                animation-duration: 2.767644001s;
                animation-delay: -2.7950220038s;
            }

            bokeh:nth-child(28) {
                background-color: #ef8d22;
                transform: translate(75.1070545511vw, 54.2036989448vh);
                animation-duration: 4.7036199387s;
                animation-delay: -1.0505926433s;
            }

            bokeh:nth-child(29) {
                background-color: #fc85e1;
                transform: translate(25.2485702636vw, 35.8851684261vh);
                animation-duration: 3.7316305594s;
                animation-delay: -1.828910888s;
            }

            bokeh:nth-child(30) {
                background-color: #2bd8ff;
                transform: translate(33.607420868vw, 8.2345981698vh);
                animation-duration: 2.7029717368s;
                animation-delay: -2.5500282063s;
            }

            bokeh:nth-child(31) {
                background-color: #fc85e1;
                transform: translate(4.5567738711vw, 26.915212362vh);
                animation-duration: 3.4355180075s;
                animation-delay: -0.5790819766s;
            }

            bokeh:nth-child(32) {
                background-color: #feff28;
                transform: translate(25.9501588313vw, 20.9473646869vh);
                animation-duration: 4.3830077577s;
                animation-delay: -4.6564701835s;
            }

            bokeh:nth-child(33) {
                background-color: #feff28;
                transform: translate(90.303759829vw, 29.6733774558vh);
                animation-duration: 2.6689654722s;
                animation-delay: -0.9045308203s;
            }

            bokeh:nth-child(34) {
                background-color: #2bd8ff;
                transform: translate(89.2836951603vw, 26.5025411567vh);
                animation-duration: 2.6426834256s;
                animation-delay: -4.8319924428s;
            }

            bokeh:nth-child(35) {
                background-color: #ef8d22;
                transform: translate(49.6593402454vw, 41.2989731288vh);
                animation-duration: 2.53627768s;
                animation-delay: -1.6992049899s;
            }

            bokeh:nth-child(36) {
                background-color: #ef8d22;
                transform: translate(55.3578105489vw, 75.1503457961vh);
                animation-duration: 2.9803742064s;
                animation-delay: -3.860230436s;
            }

            bokeh:nth-child(37) {
                background-color: #feff28;
                transform: translate(84.2137545181vw, 99.6489820089vh);
                animation-duration: 2.8525129053s;
                animation-delay: -1.909336042s;
            }

            bokeh:nth-child(38) {
                background-color: #feff28;
                transform: translate(58.4226829219vw, 6.6082231423vh);
                animation-duration: 4.1724251653s;
                animation-delay: -2.5373921442s;
            }

            bokeh:nth-child(39) {
                background-color: #2bd8ff;
                transform: translate(4.1325762908vw, 16.5826905712vh);
                animation-duration: 3.3196820224s;
                animation-delay: -0.1998524335s;
            }

            bokeh:nth-child(40) {
                background-color: #ef8d22;
                transform: translate(38.1082612566vw, 99.6828149038vh);
                animation-duration: 2.4716860672s;
                animation-delay: -3.804687821s;
            }

            bokeh:nth-child(41) {
                background-color: #ef8d22;
                transform: translate(80.1246196199vw, 23.2154454066vh);
                animation-duration: 3.9966714491s;
                animation-delay: -3.2041854036s;
            }

            bokeh:nth-child(42) {
                background-color: #2bd8ff;
                transform: translate(12.4867607956vw, 81.990153671vh);
                animation-duration: 4.3771268993s;
                animation-delay: -2.9204017862s;
            }

            bokeh:nth-child(43) {
                background-color: #feff28;
                transform: translate(88.4304689846vw, 21.1509289349vh);
                animation-duration: 2.4345176476s;
                animation-delay: -1.7879472609s;
            }

            bokeh:nth-child(44) {
                background-color: #fc85e1;
                transform: translate(69.7647889352vw, 45.9607535566vh);
                animation-duration: 4.3935398987s;
                animation-delay: -3.4611102331s;
            }

            bokeh:nth-child(45) {
                background-color: #ef8d22;
                transform: translate(61.1024281766vw, 8.6360893002vh);
                animation-duration: 3.7418427756s;
                animation-delay: -0.8676250685s;
            }

            bokeh:nth-child(46) {
                background-color: #2bd8ff;
                transform: translate(3.2214371062vw, 25.2935105902vh);
                animation-duration: 3.074683766s;
                animation-delay: -0.4965853318s;
            }

            bokeh:nth-child(47) {
                background-color: #feff28;
                transform: translate(74.1716691607vw, 3.1894365936vh);
                animation-duration: 4.4907628187s;
                animation-delay: -2.968930085s;
            }

            bokeh:nth-child(48) {
                background-color: #fc85e1;
                transform: translate(71.7485884871vw, 81.5140808668vh);
                animation-duration: 4.6478212704s;
                animation-delay: -2.4913789916s;
            }

            bokeh:nth-child(49) {
                background-color: #ef8d22;
                transform: translate(68.5706834892vw, 26.9999891094vh);
                animation-duration: 4.4816990552s;
                animation-delay: -4.3381289066s;
            }

            bokeh:nth-child(50) {
                background-color: #ef8d22;
                transform: translate(41.4062073866vw, 53.7404657598vh);
                animation-duration: 3.4662897168s;
                animation-delay: -3.0623966223s;
            }

            bokeh:nth-child(51) {
                background-color: #ef8d22;
                transform: translate(87.7275522899vw, 57.8586420239vh);
                animation-duration: 4.5492821401s;
                animation-delay: -3.9375445372s;
            }

            bokeh:nth-child(52) {
                background-color: #fc85e1;
                transform: translate(98.2142162683vw, 57.3579443658vh);
                animation-duration: 2.8023852526s;
                animation-delay: -2.8018360542s;
            }

            bokeh:nth-child(53) {
                background-color: #ef8d22;
                transform: translate(58.9158153095vw, 2.5851120782vh);
                animation-duration: 4.8828427898s;
                animation-delay: -4.0170178676s;
            }

            bokeh:nth-child(54) {
                background-color: #feff28;
                transform: translate(21.8232629797vw, 30.541333487vh);
                animation-duration: 4.1215064165s;
                animation-delay: -1.7175877986s;
            }

            bokeh:nth-child(55) {
                background-color: #fc85e1;
                transform: translate(13.5806715283vw, 97.9236982484vh);
                animation-duration: 3.5107176799s;
                animation-delay: -2.201395581s;
            }

            bokeh:nth-child(56) {
                background-color: #feff28;
                transform: translate(14.4730253941vw, 70.3026987242vh);
                animation-duration: 2.8655370997s;
                animation-delay: -4.5406682184s;
            }

            bokeh:nth-child(57) {
                background-color: #feff28;
                transform: translate(8.9309655313vw, 17.5932162599vh);
                animation-duration: 3.8738411593s;
                animation-delay: -0.7726217596s;
            }

            bokeh:nth-child(58) {
                background-color: #fc85e1;
                transform: translate(37.5050301898vw, 74.5977925362vh);
                animation-duration: 2.8543587537s;
                animation-delay: -0.6382727009s;
            }

            bokeh:nth-child(59) {
                background-color: #fc85e1;
                transform: translate(44.1369706808vw, 19.0224357251vh);
                animation-duration: 3.4677241213s;
                animation-delay: -0.3790625881s;
            }

            bokeh:nth-child(60) {
                background-color: #ef8d22;
                transform: translate(89.9172143086vw, 60.5896372203vh);
                animation-duration: 2.2591286422s;
                animation-delay: -3.3436293949s;
            }

            bokeh:nth-child(61) {
                background-color: #2bd8ff;
                transform: translate(86.129997629vw, 57.7175593668vh);
                animation-duration: 3.3394070906s;
                animation-delay: -1.2058207724s;
            }

            bokeh:nth-child(62) {
                background-color: #ef8d22;
                transform: translate(62.6094040216vw, 64.6028247058vh);
                animation-duration: 2.7708027023s;
                animation-delay: -1.3248560361s;
            }

            bokeh:nth-child(63) {
                background-color: #fc85e1;
                transform: translate(1.4935870167vw, 49.1580693638vh);
                animation-duration: 4.0753471222s;
                animation-delay: -1.1042384607s;
            }

            bokeh:nth-child(64) {
                background-color: #ef8d22;
                transform: translate(49.4229799547vw, 14.4558125829vh);
                animation-duration: 4.6042743538s;
                animation-delay: -1.5068368619s;
            }

            bokeh:nth-child(65) {
                background-color: #2bd8ff;
                transform: translate(24.1752717226vw, 44.959300202vh);
                animation-duration: 2.7140677085s;
                animation-delay: -4.1288509334s;
            }

            bokeh:nth-child(66) {
                background-color: #2bd8ff;
                transform: translate(47.8734263303vw, 94.391925096vh);
                animation-duration: 4.5332114735s;
                animation-delay: -2.9163200431s;
            }

            bokeh:nth-child(67) {
                background-color: #ef8d22;
                transform: translate(78.8655189976vw, 86.980092905vh);
                animation-duration: 2.3004360444s;
                animation-delay: -2.2638107753s;
            }

            bokeh:nth-child(68) {
                background-color: #feff28;
                transform: translate(9.900688433vw, 44.1486399622vh);
                animation-duration: 4.5713456324s;
                animation-delay: -1.6496695177s;
            }

            bokeh:nth-child(69) {
                background-color: #fc85e1;
                transform: translate(69.5673498579vw, 22.4102469728vh);
                animation-duration: 4.5195536497s;
                animation-delay: -2.4477867877s;
            }

            bokeh:nth-child(70) {
                background-color: #fc85e1;
                transform: translate(11.1928628475vw, 56.5732657592vh);
                animation-duration: 4.2452477565s;
                animation-delay: -4.784497837s;
            }

            bokeh:nth-child(71) {
                background-color: #feff28;
                transform: translate(55.2490898496vw, 28.0060803314vh);
                animation-duration: 2.4738318304s;
                animation-delay: -4.2575550351s;
            }

            bokeh:nth-child(72) {
                background-color: #ef8d22;
                transform: translate(47.5206781163vw, 98.1803905721vh);
                animation-duration: 4.4299041867s;
                animation-delay: -1.6544913646s;
            }

            bokeh:nth-child(73) {
                background-color: #fc85e1;
                transform: translate(3.3800457033vw, 87.8857972808vh);
                animation-duration: 2.1543860283s;
                animation-delay: -1.5361790929s;
            }

            bokeh:nth-child(74) {
                background-color: #feff28;
                transform: translate(50.2022983803vw, 53.6621206454vh);
                animation-duration: 3.5498075114s;
                animation-delay: -1.622928478s;
            }

            bokeh:nth-child(75) {
                background-color: #2bd8ff;
                transform: translate(61.4792038272vw, 49.9574099775vh);
                animation-duration: 4.3023511502s;
                animation-delay: -2.5662268689s;
            }

            bokeh:nth-child(76) {
                background-color: #2bd8ff;
                transform: translate(96.8566584025vw, 62.4294941633vh);
                animation-duration: 3.0488542535s;
                animation-delay: -3.2247802825s;
            }

            bokeh:nth-child(77) {
                background-color: #ef8d22;
                transform: translate(39.2082016768vw, 31.510327441vh);
                animation-duration: 3.3263311044s;
                animation-delay: -4.8680742107s;
            }

            bokeh:nth-child(78) {
                background-color: #ef8d22;
                transform: translate(96.5195887397vw, 10.3731475626vh);
                animation-duration: 4.2409467825s;
                animation-delay: -0.7158376764s;
            }

            bokeh:nth-child(79) {
                background-color: #fc85e1;
                transform: translate(60.3099737688vw, 98.3753373411vh);
                animation-duration: 2.5537973442s;
                animation-delay: -0.63998392s;
            }

            bokeh:nth-child(80) {
                background-color: #ef8d22;
                transform: translate(11.5967388759vw, 14.9299043275vh);
                animation-duration: 2.8098590221s;
                animation-delay: -2.4370859968s;
            }

            bokeh:nth-child(81) {
                background-color: #ef8d22;
                transform: translate(74.1223777298vw, 70.1971631522vh);
                animation-duration: 4.2838589963s;
                animation-delay: -3.7401444523s;
            }

            bokeh:nth-child(82) {
                background-color: #feff28;
                transform: translate(84.1015262739vw, 81.3441360981vh);
                animation-duration: 3.2939592107s;
                animation-delay: -1.9150983315s;
            }

            bokeh:nth-child(83) {
                background-color: #fc85e1;
                transform: translate(0.7106752653vw, 36.7850329091vh);
                animation-duration: 4.8849572533s;
                animation-delay: -1.6034485131s;
            }

            bokeh:nth-child(84) {
                background-color: #ef8d22;
                transform: translate(87.8717119902vw, 89.8137587323vh);
                animation-duration: 4.4917909367s;
                animation-delay: -0.6839290268s;
            }

            bokeh:nth-child(85) {
                background-color: #fc85e1;
                transform: translate(57.2928640388vw, 75.8426881671vh);
                animation-duration: 3.1987712966s;
                animation-delay: -0.7031902792s;
            }

            bokeh:nth-child(86) {
                background-color: #fc85e1;
                transform: translate(95.0682843643vw, 18.2581374607vh);
                animation-duration: 2.8925956423s;
                animation-delay: -1.0572694348s;
            }

            bokeh:nth-child(87) {
                background-color: #fc85e1;
                transform: translate(59.0707981851vw, 48.7661464606vh);
                animation-duration: 2.6026617399s;
                animation-delay: -4.8628976688s;
            }

            bokeh:nth-child(88) {
                background-color: #fc85e1;
                transform: translate(41.8052009135vw, 3.1629584265vh);
                animation-duration: 3.9945698031s;
                animation-delay: -3.2234605093s;
            }

            bokeh:nth-child(89) {
                background-color: #2bd8ff;
                transform: translate(47.1542426485vw, 6.2335870209vh);
                animation-duration: 3.2101759535s;
                animation-delay: -4.3446493263s;
            }

            bokeh:nth-child(90) {
                background-color: #feff28;
                transform: translate(55.1752701425vw, 47.3028980994vh);
                animation-duration: 3.7706786674s;
                animation-delay: -3.1945484167s;
            }

            bokeh:nth-child(91) {
                background-color: #2bd8ff;
                transform: translate(64.3680183118vw, 70.2328105992vh);
                animation-duration: 4.9905256372s;
                animation-delay: -3.3445529913s;
            }

            bokeh:nth-child(92) {
                background-color: #fc85e1;
                transform: translate(57.1140237902vw, 90.0487890223vh);
                animation-duration: 3.8901112768s;
                animation-delay: -1.6312829089s;
            }

            bokeh:nth-child(93) {
                background-color: #feff28;
                transform: translate(79.8479180254vw, 50.5459436949vh);
                animation-duration: 2.0763765466s;
                animation-delay: -2.2578885579s;
            }

            bokeh:nth-child(94) {
                background-color: #feff28;
                transform: translate(19.6698287233vw, 25.3724994599vh);
                animation-duration: 2.3036069206s;
                animation-delay: -4.4809995763s;
            }

            bokeh:nth-child(95) {
                background-color: #fc85e1;
                transform: translate(53.2976851652vw, 47.9411811828vh);
                animation-duration: 4.0118610481s;
                animation-delay: -4.5248562455s;
            }

            bokeh:nth-child(96) {
                background-color: #feff28;
                transform: translate(39.9679535656vw, 74.256254716vh);
                animation-duration: 3.4959949039s;
                animation-delay: -3.4307375377s;
            }

            bokeh:nth-child(97) {
                background-color: #feff28;
                transform: translate(22.0090368657vw, 87.5674469503vh);
                animation-duration: 2.1309873931s;
                animation-delay: -2.9910336889s;
            }

            bokeh:nth-child(98) {
                background-color: #ef8d22;
                transform: translate(19.475671768vw, 52.8257337375vh);
                animation-duration: 2.0885845263s;
                animation-delay: -3.3263154797s;
            }

            bokeh:nth-child(99) {
                background-color: #ef8d22;
                transform: translate(64.559290293vw, 91.8668029819vh);
                animation-duration: 4.6404932212s;
                animation-delay: -4.9311549742s;
            }

            bokeh:nth-child(100) {
                background-color: #fc85e1;
                transform: translate(23.7654664572vw, 23.0565546063vh);
                animation-duration: 2.4373894218s;
                animation-delay: -3.7747104339s;
            }

            @keyframes explosion {
                0% {
                    opacity: 0;
                }
                70% {
                    opacity: 1;
                }
                100% {
                    transform: translate(50vw, 100vh);
                }
            }
            .cake {
                position: relative;
                top: 350px;
                margin: auto;
                width: 200px;
                height: 60px;
                background: #f9fdff;
                border-radius: 100%;
                transform: translateZ(100px);
                box-shadow: 0px 4px 0px #f4f9fd, 0px 8px 0px #dba9ff, 0px 12px 0px #fec3b3, 0px 16px 0px #f7f6fb, 0px 20px 0px #f7f6fb, 0px 24px 0px #f7f6fb, 0px 28px 0px #f7f6fb, 0px 32px 0px #fea0bb, 0px 36px 0px #fea0bb, 0px 40px 0px #9cef9d, 0px 44px 0px #9cef9d, 0px 48px 0px #f7f6fb, 0px 52px 0px #f7f6fb, 0px 56px 0px #f7f6fb, 0px 60px 0px #f7f6fb, 0px 64px 0px #f7f6fb, 0px 68px 0px #dfa5fc, 0px 72px 0px #dfa5fc, 0px 76px 0px #fafffe, 0px 80px 0px #fafffe;
            }

            .plate {
                position: absolute;
                height: 90px;
                width: 300px;
                bottom: -95px;
                left: 50%;
                top: 480px;
                margin-left: -150px;
                border-radius: 100%;
                background: radial-gradient(ellipse closest-side at center, #08c7fe 0%, #04d7f2 71%, #02ffd0 100%);
                box-shadow: 0px 3px 0px #00e2e1, 0px 6px 0px #00d3fb;
                transform: translateZ(80px);
            }

            .candle {
                position: relative;
                height: 50px;
                width: 12px;
                top: 380px;
                margin: auto;
                background: linear-gradient(0deg, #b7f4a7 0%, white 100%);
                border-radius: 4px;
                transform: translateZ(120px);
            }

            #flame {
                position: absolute;
                z-index: 10;
            }

            .lit {
                background: linear-gradient(to bottom, #FFF6D9, #FBC36C);
                width: 15px;
                height: 35px;
                /*  Info on border radius. http://www.css3.info/preview/rounded-border/ */
                border-top-left-radius: 10px 35px;
                border-top-right-radius: 10px 35px;
                border-bottom-right-radius: 10px 10px;
                border-bottom-left-radius: 10px 10px;
                top: -34px;
                margin: auto;
                /*   http://www.css3.info/preview/box-shadow/ */
                box-shadow: 0 0 17px 7px rgba(251, 246, 190, 0.71);
                transform-origin: bottom;
                animation: flicker 1s ease-in-out alternate infinite;
            }

            @keyframes flicker {
                0% {
                    transform: skewX(5deg);
                    box-shadow: 0 0 17px 10px rgba(251, 246, 190, 0.71);
                }
                25% {
                    transform: skewX(-5deg);
                    box-shadow: 0 0 17px 5px rgba(251, 246, 190, 0.71);
                }
                50% {
                    transform: skewX(10deg);
                    box-shadow: 0 0 17px 7px rgba(251, 246, 190, 0.71);
                }
                75% {
                    transform: skewX(-10deg);
                    box-shadow: 0 0 17px 5px rgba(251, 246, 190, 0.71);
                }
                100% {
                    transform: skewX(5deg);
                    box-shadow: 0 0 17px 10px rgba(251, 246, 190, 0.71);
                }
            }
            .pyro > .before, .pyro > .after {
                position: fixed;
                width: 5px;
                height: 5px;
                border-radius: 50%;
                box-shadow: 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff, 0 0 #fff;
                -moz-animation: 1s bang ease-out infinite backwards, 1s gravity ease-in infinite backwards, 5s position linear infinite backwards;
                -webkit-animation: 1s bang ease-out infinite backwards, 1s gravity ease-in infinite backwards, 5s position linear infinite backwards;
                -o-animation: 1s bang ease-out infinite backwards, 1s gravity ease-in infinite backwards, 5s position linear infinite backwards;
                -ms-animation: 1s bang ease-out infinite backwards, 1s gravity ease-in infinite backwards, 5s position linear infinite backwards;
                animation: 1s bang ease-out infinite backwards, 1s gravity ease-in infinite backwards, 5s position linear infinite backwards;
            }

            .pyro > .after {
                -moz-animation-delay: 1.25s, 1.25s, 1.25s;
                -webkit-animation-delay: 1.25s, 1.25s, 1.25s;
                -o-animation-delay: 1.25s, 1.25s, 1.25s;
                -ms-animation-delay: 1.25s, 1.25s, 1.25s;
                animation-delay: 1.25s, 1.25s, 1.25s;
                -moz-animation-duration: 1.25s, 1.25s, 6.25s;
                -webkit-animation-duration: 1.25s, 1.25s, 6.25s;
                -o-animation-duration: 1.25s, 1.25s, 6.25s;
                -ms-animation-duration: 1.25s, 1.25s, 6.25s;
                animation-duration: 1.25s, 1.25s, 6.25s;
            }

            @-webkit-keyframes bang {
                to {
                    box-shadow: -110px -104.6666666667px #00ff51, -3px 36.3333333333px #5eff00, 249px -295.6666666667px #00ff84, -165px -32.6666666667px #ff00e6, 49px -14.6666666667px #ff6600, -2px -370.6666666667px #00ddff, 60px -245.6666666667px #ddff00, 135px -205.6666666667px #00a6ff, 139px -204.6666666667px #ff00fb, -36px -155.6666666667px #00ff48, -75px 8.3333333333px #00ff84, -202px -139.6666666667px #00ff0d, 123px -84.6666666667px #00ffaa, 37px -396.6666666667px #6aff00, -157px -134.6666666667px #ff5900, 7px 6.3333333333px #ffbb00, 222px -15.6666666667px #66ff00, -114px -40.6666666667px #ffb700, -127px -49.6666666667px #ffb300, 130px -63.6666666667px #0080ff, 139px -11.6666666667px #0077ff, -167px -301.6666666667px #ff00e6, 55px -222.6666666667px #62ff00, 12px -10.6666666667px #95ff00, -240px -114.6666666667px #ff9900, -78px -210.6666666667px blue, 175px -142.6666666667px #3700ff, 83px -316.6666666667px #ff00c4, 69px -390.6666666667px #ff0040, -168px -361.6666666667px #00aaff, -44px -87.6666666667px #0040ff, 235px -415.6666666667px #ffae00, 45px 55.3333333333px #00ff0d, -61px -2.6666666667px #e600ff, -225px -59.6666666667px #59ff00, -30px 48.3333333333px #00f7ff, 211px -170.6666666667px #f700ff, -165px -209.6666666667px #37ff00, -131px -306.6666666667px #00ff66, -137px 54.3333333333px red, 42px -397.6666666667px #00e1ff, 230px -250.6666666667px #ff4d00, -172px -335.6666666667px #000dff, 143px -342.6666666667px #04ff00, -76px -194.6666666667px #fff200, -237px -166.6666666667px #00a6ff, -172px -178.6666666667px #d0ff00, 51px -72.6666666667px #1500ff, -206px 34.3333333333px #ff0015, 51px 11.3333333333px #ff0400, -149px -215.6666666667px #ff0048;
                }
            }
            @-moz-keyframes bang {
                to {
                    box-shadow: -110px -104.6666666667px #00ff51, -3px 36.3333333333px #5eff00, 249px -295.6666666667px #00ff84, -165px -32.6666666667px #ff00e6, 49px -14.6666666667px #ff6600, -2px -370.6666666667px #00ddff, 60px -245.6666666667px #ddff00, 135px -205.6666666667px #00a6ff, 139px -204.6666666667px #ff00fb, -36px -155.6666666667px #00ff48, -75px 8.3333333333px #00ff84, -202px -139.6666666667px #00ff0d, 123px -84.6666666667px #00ffaa, 37px -396.6666666667px #6aff00, -157px -134.6666666667px #ff5900, 7px 6.3333333333px #ffbb00, 222px -15.6666666667px #66ff00, -114px -40.6666666667px #ffb700, -127px -49.6666666667px #ffb300, 130px -63.6666666667px #0080ff, 139px -11.6666666667px #0077ff, -167px -301.6666666667px #ff00e6, 55px -222.6666666667px #62ff00, 12px -10.6666666667px #95ff00, -240px -114.6666666667px #ff9900, -78px -210.6666666667px blue, 175px -142.6666666667px #3700ff, 83px -316.6666666667px #ff00c4, 69px -390.6666666667px #ff0040, -168px -361.6666666667px #00aaff, -44px -87.6666666667px #0040ff, 235px -415.6666666667px #ffae00, 45px 55.3333333333px #00ff0d, -61px -2.6666666667px #e600ff, -225px -59.6666666667px #59ff00, -30px 48.3333333333px #00f7ff, 211px -170.6666666667px #f700ff, -165px -209.6666666667px #37ff00, -131px -306.6666666667px #00ff66, -137px 54.3333333333px red, 42px -397.6666666667px #00e1ff, 230px -250.6666666667px #ff4d00, -172px -335.6666666667px #000dff, 143px -342.6666666667px #04ff00, -76px -194.6666666667px #fff200, -237px -166.6666666667px #00a6ff, -172px -178.6666666667px #d0ff00, 51px -72.6666666667px #1500ff, -206px 34.3333333333px #ff0015, 51px 11.3333333333px #ff0400, -149px -215.6666666667px #ff0048;
                }
            }
            @-o-keyframes bang {
                to {
                    box-shadow: -110px -104.6666666667px #00ff51, -3px 36.3333333333px #5eff00, 249px -295.6666666667px #00ff84, -165px -32.6666666667px #ff00e6, 49px -14.6666666667px #ff6600, -2px -370.6666666667px #00ddff, 60px -245.6666666667px #ddff00, 135px -205.6666666667px #00a6ff, 139px -204.6666666667px #ff00fb, -36px -155.6666666667px #00ff48, -75px 8.3333333333px #00ff84, -202px -139.6666666667px #00ff0d, 123px -84.6666666667px #00ffaa, 37px -396.6666666667px #6aff00, -157px -134.6666666667px #ff5900, 7px 6.3333333333px #ffbb00, 222px -15.6666666667px #66ff00, -114px -40.6666666667px #ffb700, -127px -49.6666666667px #ffb300, 130px -63.6666666667px #0080ff, 139px -11.6666666667px #0077ff, -167px -301.6666666667px #ff00e6, 55px -222.6666666667px #62ff00, 12px -10.6666666667px #95ff00, -240px -114.6666666667px #ff9900, -78px -210.6666666667px blue, 175px -142.6666666667px #3700ff, 83px -316.6666666667px #ff00c4, 69px -390.6666666667px #ff0040, -168px -361.6666666667px #00aaff, -44px -87.6666666667px #0040ff, 235px -415.6666666667px #ffae00, 45px 55.3333333333px #00ff0d, -61px -2.6666666667px #e600ff, -225px -59.6666666667px #59ff00, -30px 48.3333333333px #00f7ff, 211px -170.6666666667px #f700ff, -165px -209.6666666667px #37ff00, -131px -306.6666666667px #00ff66, -137px 54.3333333333px red, 42px -397.6666666667px #00e1ff, 230px -250.6666666667px #ff4d00, -172px -335.6666666667px #000dff, 143px -342.6666666667px #04ff00, -76px -194.6666666667px #fff200, -237px -166.6666666667px #00a6ff, -172px -178.6666666667px #d0ff00, 51px -72.6666666667px #1500ff, -206px 34.3333333333px #ff0015, 51px 11.3333333333px #ff0400, -149px -215.6666666667px #ff0048;
                }
            }
            @-ms-keyframes bang {
                to {
                    box-shadow: -110px -104.6666666667px #00ff51, -3px 36.3333333333px #5eff00, 249px -295.6666666667px #00ff84, -165px -32.6666666667px #ff00e6, 49px -14.6666666667px #ff6600, -2px -370.6666666667px #00ddff, 60px -245.6666666667px #ddff00, 135px -205.6666666667px #00a6ff, 139px -204.6666666667px #ff00fb, -36px -155.6666666667px #00ff48, -75px 8.3333333333px #00ff84, -202px -139.6666666667px #00ff0d, 123px -84.6666666667px #00ffaa, 37px -396.6666666667px #6aff00, -157px -134.6666666667px #ff5900, 7px 6.3333333333px #ffbb00, 222px -15.6666666667px #66ff00, -114px -40.6666666667px #ffb700, -127px -49.6666666667px #ffb300, 130px -63.6666666667px #0080ff, 139px -11.6666666667px #0077ff, -167px -301.6666666667px #ff00e6, 55px -222.6666666667px #62ff00, 12px -10.6666666667px #95ff00, -240px -114.6666666667px #ff9900, -78px -210.6666666667px blue, 175px -142.6666666667px #3700ff, 83px -316.6666666667px #ff00c4, 69px -390.6666666667px #ff0040, -168px -361.6666666667px #00aaff, -44px -87.6666666667px #0040ff, 235px -415.6666666667px #ffae00, 45px 55.3333333333px #00ff0d, -61px -2.6666666667px #e600ff, -225px -59.6666666667px #59ff00, -30px 48.3333333333px #00f7ff, 211px -170.6666666667px #f700ff, -165px -209.6666666667px #37ff00, -131px -306.6666666667px #00ff66, -137px 54.3333333333px red, 42px -397.6666666667px #00e1ff, 230px -250.6666666667px #ff4d00, -172px -335.6666666667px #000dff, 143px -342.6666666667px #04ff00, -76px -194.6666666667px #fff200, -237px -166.6666666667px #00a6ff, -172px -178.6666666667px #d0ff00, 51px -72.6666666667px #1500ff, -206px 34.3333333333px #ff0015, 51px 11.3333333333px #ff0400, -149px -215.6666666667px #ff0048;
                }
            }
            @keyframes bang {
                to {
                    box-shadow: -110px -104.6666666667px #00ff51, -3px 36.3333333333px #5eff00, 249px -295.6666666667px #00ff84, -165px -32.6666666667px #ff00e6, 49px -14.6666666667px #ff6600, -2px -370.6666666667px #00ddff, 60px -245.6666666667px #ddff00, 135px -205.6666666667px #00a6ff, 139px -204.6666666667px #ff00fb, -36px -155.6666666667px #00ff48, -75px 8.3333333333px #00ff84, -202px -139.6666666667px #00ff0d, 123px -84.6666666667px #00ffaa, 37px -396.6666666667px #6aff00, -157px -134.6666666667px #ff5900, 7px 6.3333333333px #ffbb00, 222px -15.6666666667px #66ff00, -114px -40.6666666667px #ffb700, -127px -49.6666666667px #ffb300, 130px -63.6666666667px #0080ff, 139px -11.6666666667px #0077ff, -167px -301.6666666667px #ff00e6, 55px -222.6666666667px #62ff00, 12px -10.6666666667px #95ff00, -240px -114.6666666667px #ff9900, -78px -210.6666666667px blue, 175px -142.6666666667px #3700ff, 83px -316.6666666667px #ff00c4, 69px -390.6666666667px #ff0040, -168px -361.6666666667px #00aaff, -44px -87.6666666667px #0040ff, 235px -415.6666666667px #ffae00, 45px 55.3333333333px #00ff0d, -61px -2.6666666667px #e600ff, -225px -59.6666666667px #59ff00, -30px 48.3333333333px #00f7ff, 211px -170.6666666667px #f700ff, -165px -209.6666666667px #37ff00, -131px -306.6666666667px #00ff66, -137px 54.3333333333px red, 42px -397.6666666667px #00e1ff, 230px -250.6666666667px #ff4d00, -172px -335.6666666667px #000dff, 143px -342.6666666667px #04ff00, -76px -194.6666666667px #fff200, -237px -166.6666666667px #00a6ff, -172px -178.6666666667px #d0ff00, 51px -72.6666666667px #1500ff, -206px 34.3333333333px #ff0015, 51px 11.3333333333px #ff0400, -149px -215.6666666667px #ff0048;
                }
            }
            @-webkit-keyframes gravity {
                to {
                    transform: translateY(200px);
                    -moz-transform: translateY(200px);
                    -webkit-transform: translateY(200px);
                    -o-transform: translateY(200px);
                    -ms-transform: translateY(200px);
                    opacity: 0;
                }
            }
            @-moz-keyframes gravity {
                to {
                    transform: translateY(200px);
                    -moz-transform: translateY(200px);
                    -webkit-transform: translateY(200px);
                    -o-transform: translateY(200px);
                    -ms-transform: translateY(200px);
                    opacity: 0;
                }
            }
            @-o-keyframes gravity {
                to {
                    transform: translateY(200px);
                    -moz-transform: translateY(200px);
                    -webkit-transform: translateY(200px);
                    -o-transform: translateY(200px);
                    -ms-transform: translateY(200px);
                    opacity: 0;
                }
            }
            @-ms-keyframes gravity {
                to {
                    transform: translateY(200px);
                    -moz-transform: translateY(200px);
                    -webkit-transform: translateY(200px);
                    -o-transform: translateY(200px);
                    -ms-transform: translateY(200px);
                    opacity: 0;
                }
            }
            @keyframes gravity {
                to {
                    transform: translateY(200px);
                    -moz-transform: translateY(200px);
                    -webkit-transform: translateY(200px);
                    -o-transform: translateY(200px);
                    -ms-transform: translateY(200px);
                    opacity: 0;
                }
            }
            @-webkit-keyframes position {
                0%, 19.9% {
                    margin-top: 10%;
                    margin-left: 40%;
                }
                20%, 39.9% {
                    margin-top: 40%;
                    margin-left: 30%;
                }
                40%, 59.9% {
                    margin-top: 20%;
                    margin-left: 70%;
                }
                60%, 79.9% {
                    margin-top: 30%;
                    margin-left: 20%;
                }
                80%, 99.9% {
                    margin-top: 30%;
                    margin-left: 80%;
                }
            }
            @-moz-keyframes position {
                0%, 19.9% {
                    margin-top: 10%;
                    margin-left: 40%;
                }
                20%, 39.9% {
                    margin-top: 40%;
                    margin-left: 30%;
                }
                40%, 59.9% {
                    margin-top: 20%;
                    margin-left: 70%;
                }
                60%, 79.9% {
                    margin-top: 30%;
                    margin-left: 20%;
                }
                80%, 99.9% {
                    margin-top: 30%;
                    margin-left: 80%;
                }
            }
            @-o-keyframes position {
                0%, 19.9% {
                    margin-top: 10%;
                    margin-left: 40%;
                }
                20%, 39.9% {
                    margin-top: 40%;
                    margin-left: 30%;
                }
                40%, 59.9% {
                    margin-top: 20%;
                    margin-left: 70%;
                }
                60%, 79.9% {
                    margin-top: 30%;
                    margin-left: 20%;
                }
                80%, 99.9% {
                    margin-top: 30%;
                    margin-left: 80%;
                }
            }
            @-ms-keyframes position {
                0%, 19.9% {
                    margin-top: 10%;
                    margin-left: 40%;
                }
                20%, 39.9% {
                    margin-top: 40%;
                    margin-left: 30%;
                }
                40%, 59.9% {
                    margin-top: 20%;
                    margin-left: 70%;
                }
                60%, 79.9% {
                    margin-top: 30%;
                    margin-left: 20%;
                }
                80%, 99.9% {
                    margin-top: 30%;
                    margin-left: 80%;
                }
            }
            @keyframes position {
                0%, 19.9% {
                    margin-top: 10%;
                    margin-left: 40%;
                }
                20%, 39.9% {
                    margin-top: 40%;
                    margin-left: 30%;
                }
                40%, 59.9% {
                    margin-top: 20%;
                    margin-left: 70%;
                }
                60%, 79.9% {
                    margin-top: 30%;
                    margin-left: 20%;
                }
                80%, 99.9% {
                    margin-top: 30%;
                    margin-left: 80%;
                }
            }
        }
    </style>
</head>
<body>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<bokeh></bokeh>
<div class="mobile">最大化查看</div>
<div class="pyro">
    <div class="before"></div>
    <div class="after"></div>
</div>
<h3>xxx，生日快乐!</h3>
<audio autoplay="autoplay" loop="loop" id="audios" preload="auto" hidden>
    <source src="file/happy.mp3"/>
</audio>
<span>🎉</span>
<div class="candle">
    <div id="flame" class="lit"></div>
</div>
<div class="cake"></div>
<div class="plate"></div>
<div style="margin-top: 550px;text-align: center;align-content: center;">
    <img src="image/shouxing.png">
</div>
</body>
</html>


