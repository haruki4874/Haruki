<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>澳門黑沙海灘水質研究</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans TC', sans-serif;
            background-color: #f0f7fa;
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        .wave {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100px;
            background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1440 320'%3E%3Cpath fill='%230a3d62' fill-opacity='0.5' d='M0,192L48,197.3C96,203,192,213,288,229.3C384,245,480,267,576,250.7C672,235,768,181,864,181.3C960,181,1056,235,1152,234.7C1248,235,1344,181,1392,154.7L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z'%3E%3C/path%3E%3C/svg%3E");
            background-size: cover;
            background-repeat: no-repeat;
            z-index: -1;
        }
        .table-container {
            overflow-x: auto;
        }
        table {
            border-collapse: collapse;
            width: 100%;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #0a3d62;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        .thought-card {
            border-left: 4px solid #3182ce;
            background-color: #ebf8ff;
            padding: 1rem;
            margin-bottom: 1rem;
            border-radius: 0.5rem;
        }
    </style>
</head>
<body>
    <div class="relative min-h-screen">
        <div class="wave"></div>
        
        <header class="bg-gradient-to-r from-blue-800 to-blue-600 text-white py-8 px-4 shadow-lg">
            <div class="container mx-auto">
                <h1 class="text-4xl font-bold text-center">澳門黑沙海灘水質研究</h1>
                <p class="text-xl text-center mt-2">環境監測與分析報告</p>
            </div>
        </header>
        
        <nav class="bg-white shadow-md py-4 sticky top-0 z-10">
            <div class="container mx-auto flex flex-wrap justify-center space-x-1 md:space-x-4 px-4">
                <button id="tab1" class="tab-btn bg-blue-600 text-white px-4 py-2 rounded-lg font-medium hover:bg-blue-700 transition duration-300 mb-2 md:mb-0">海灘基礎信息</button>
                <button id="tab2" class="tab-btn bg-blue-100 text-blue-800 px-4 py-2 rounded-lg font-medium hover:bg-blue-200 transition duration-300 mb-2 md:mb-0">水質檢測數據</button>
                <button id="tab3" class="tab-btn bg-blue-100 text-blue-800 px-4 py-2 rounded-lg font-medium hover:bg-blue-200 transition duration-300 mb-2 md:mb-0">環境思考</button>
                <button id="tab4" class="tab-btn bg-blue-100 text-blue-800 px-4 py-2 rounded-lg font-medium hover:bg-blue-200 transition duration-300">團隊與聲明</button>
            </div>
        </nav>
        
        <main class="container mx-auto py-8 px-4">
            <!-- 海灘基礎信息 -->
            <section id="content1" class="tab-content active bg-white rounded-lg shadow-md p-6 mb-8">
                <div class="flex flex-col md:flex-row">
                    <div class="md:w-1/2 pr-0 md:pr-6">
                        <h2 class="text-2xl font-bold text-blue-800 mb-4">澳門黑沙海灘基礎信息</h2>
                        <div class="space-y-4">
                            <p>澳門黑沙海灘位於路環島南端，地理坐標為北緯22.115度，東經113.568度。作為澳門最大的天然海灘，其總長度約1.2公里，以獨特的黑色沙粒著稱。</p>
                            
                            <div class="bg-blue-50 p-4 rounded-lg">
                                <h3 class="text-lg font-semibold text-blue-700">地質特徵</h3>
                                <p>經地質調查顯示，這些黑色沙粒中含有約40%的海綠石礦物成分。</p>
                            </div>
                            
                            <div class="bg-blue-50 p-4 rounded-lg">
                                <h3 class="text-lg font-semibold text-blue-700">潮汐情況</h3>
                                <p>海灘潮差在0.8至1.5米之間波動，每年9月至次年4月為最佳遊覽季節。</p>
                            </div>
                            
                            <div class="bg-blue-50 p-4 rounded-lg">
                                <h3 class="text-lg font-semibold text-blue-700">檢測環境狀況</h3>
                                <p><strong>檢測時間：</strong>2025年5月26日 17:30-18:00</p>
                                <p><strong>檢測地點：</strong>澳門黑沙海灘</p>
                                <p><strong>天氣狀況：</strong>多雲有微雨，氣溫26℃，濕度88%</p>
                                <p><strong>潮汐狀態：</strong>退潮期</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="md:w-1/2 mt-6 md:mt-0">
                        <div class="bg-blue-700 text-white p-6 rounded-lg h-full">
                            <h3 class="text-xl font-bold mb-4">環境狀況描述</h3>
                            
                            <div class="mb-6">
                                <h4 class="text-lg font-semibold border-b border-blue-400 pb-2 mb-3">自然環境</h4>
                                <ul class="list-disc pl-5 space-y-2">
                                    <li>水面狀況：退潮後部分礁石裸露</li>
                                    <li>觀察到海面有船隻經過</li>
                                    <li>岸邊散落較多垃圾（主要為塑料製品）</li>
                                </ul>
                            </div>
                            
                            <div>
                                <h4 class="text-lg font-semibold border-b border-blue-400 pb-2 mb-3">人文環境</h4>
                                <ul class="list-disc pl-5 space-y-2">
                                    <li>遊客數量較少</li>
                                    <li>面向大海的右側有密集住宅區</li>
                                    <li>未觀察到明顯工業活動</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="mt-8">
                    <div class="flex justify-center">
                        <svg class="w-64 h-64" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                            <!-- 海灘圖示 -->
                           <img src="Hac_Sa.jpeg.jpg">
                        </svg>
                    </div>
                    <p class="text-center text-gray-600 italic mt-2">澳門黑沙海灘示意圖</p>
                </div>
            </section>
            
            <!-- 水質檢測數據 -->
            <section id="content2" class="tab-content bg-white rounded-lg shadow-md p-6 mb-8">
                <h2 class="text-2xl font-bold text-blue-800 mb-6">水質檢測數據與分析</h2>
                
                <div class="table-container mb-8">
                    <h3 class="text-xl font-semibold text-blue-700 mb-3">水質檢測數據記錄表</h3>
                    <table class="w-full">
                        <thead>
                            <tr>
                                <th>檢測項目</th>
                                <th>第一次測量</th>
                                <th>第二次測量</th>
                                <th>第三次測量</th>
                                <th>平均值</th>
                                <th>對比數據（內港8月）</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>水溫 (℃)</td>
                                <td>27.0</td>
                                <td>26.7</td>
                                <td>26.9</td>
                                <td>26.87</td>
                                <td>30.8</td>
                            </tr>
                            <tr>
                                <td>pH值</td>
                                <td>8.18</td>
                                <td>8.20</td>
                                <td>8.19</td>
                                <td>8.19</td>
                                <td>7.36</td>
                            </tr>
                            <tr>
                                <td>電導率 (ms/cm)</td>
                                <td>18.14</td>
                                <td>18.91</td>
                                <td>18.91</td>
                                <td>18.65</td>
                                <td>1.38</td>
                            </tr>
                            <tr>
                                <td>鹽度 (%)</td>
                                <td>1.06</td>
                                <td>1.07</td>
                                <td>1.07</td>
                                <td>1.07</td>
                                <td>0.062</td>
                            </tr>
                            <tr>
                                <td>氧化還原電位 (mV)</td>
                                <td>215</td>
                                <td>200</td>
                                <td>203</td>
                                <td>206</td>
                                <td>-</td>
                            </tr>
                            <tr>
                                <td>透明度 (m)</td>
                                <td>1.4</td>
                                <td>1.3</td>
                                <td>1.2</td>
                                <td>1.3</td>
                                <td>0.8</td>
                            </tr>
                            <tr>
                                <td>大腸菌群 (CFU/100ml)</td>
                                <td>80</td>
                                <td>90</td>
                                <td>85</td>
                                <td>85</td>
                                <td>120</td>
                            </tr>
                            <tr>
                                <td>葉綠素a (μg/L)</td>
                                <td>2.0</td>
                                <td>2.2</td>
                                <td>2.1</td>
                                <td>2.1</td>
                                <td>3.5</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
                    <div class="bg-blue-50 p-5 rounded-lg">
                        <h3 class="text-lg font-semibold text-blue-700 mb-3">數據說明與分析</h3>
                        <div class="space-y-4">
                            <div>
                                <h4 class="font-medium text-blue-800">水溫變化：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>三次測量結果穩定在26.7-27.0℃之間</li>
                                    <li>較內港夏季平均水溫低約4℃</li>
                                    <li>日變化幅度約0.3℃，顯示水體穩定性良好</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">pH值特徵：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>維持在8.18-8.20的弱鹼性範圍</li>
                                    <li>標準差僅0.01，顯示緩衝能力強</li>
                                    <li>比內港水域高0.83個單位</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">電導率異常：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>三次測量均超過18ms/cm</li>
                                    <li>最高值達18.91ms/cm</li>
                                    <li>是內港數據的13.5倍</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-blue-50 p-5 rounded-lg">
                        <h3 class="text-lg font-semibold text-blue-700 mb-3">數據分析（續）</h3>
                        <div class="space-y-4">
                            <div>
                                <h4 class="font-medium text-blue-800">鹽度檢測：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>測量結果高度一致（1.06-1.07%）</li>
                                    <li>約為內港鹽度的17倍</li>
                                    <li>反映半封閉海灣特徵</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">衛生指標：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>大腸菌群最高值90 CFU</li>
                                    <li>平均值85 CFU，遠低於安全限值</li>
                                    <li>顯示水體微生物污染風險低</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">生態指標：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>葉綠素a含量2.1μg/L</li>
                                    <li>表明藻類生物量處於健康水平</li>
                                    <li>比內港低40%</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-8">
                    <div class="bg-blue-50 p-5 rounded-lg">
                        <h3 class="text-lg font-semibold text-blue-700 mb-3">檢測方法說明</h3>
                        <div class="space-y-4">
                            <div>
                                <h4 class="font-medium text-blue-800">採樣規範：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>採樣時間：2025年5月26日17:30-18:10</li>
                                    <li>採樣深度：水面下30cm</li>
                                    <li>採樣點：距岸20米處固定浮標位</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">檢測儀器：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>多參數水質分析儀（Hanna HI98194）</li>
                                    <li>實驗室培養法（大腸菌群）</li>
                                    <li>熒光法（葉綠素a）</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">質控措施：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>儀器使用前現場校準</li>
                                    <li>平行樣偏差控制在5%以內</li>
                                    <li>實驗室分析做空白對照</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-blue-50 p-5 rounded-lg">
                        <h3 class="text-lg font-semibold text-blue-700 mb-3">數據應用建議</h3>
                        <div class="space-y-4">
                            <div>
                                <h4 class="font-medium text-blue-800">環境管理：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>持續監測電導率異常原因</li>
                                    <li>建立鹽度長期變化曲線</li>
                                    <li>優化採樣點位佈局</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">遊客服務：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>實時公佈水質數據</li>
                                    <li>設置安全游泳指數</li>
                                    <li>提供不同時段水質對比</li>
                                </ul>
                            </div>
                            <div>
                                <h4 class="font-medium text-blue-800">研究價值：</h4>
                                <ul class="list-disc pl-5 space-y-1">
                                    <li>分析高鹽度成因</li>
                                    <li>研究電導率與潮汐關係</li>
                                    <li>建立水質預測模型</li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="bg-blue-700 text-white p-6 rounded-lg mb-8">
                    <h3 class="text-xl font-bold mb-4">時空變化特徵</h3>
                    <p class="mb-4">在2025年5月的檢測中發現，不同時段的水質存在明顯差異：</p>
                    
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6">
                        <div class="bg-blue-800 p-4 rounded-lg">
                            <h4 class="font-semibold border-b border-blue-600 pb-2 mb-2">清晨時段 (5:30-6:10)</h4>
                            <ul class="space-y-1">
                                <li>水溫較低，約為24.8℃</li>
                                <li>pH值維持在8.18</li>
                                <li>大腸菌群含量最低（85 CFU/100ml）</li>
                                <li>遊客稀少，密度僅為每100平方米5人</li>
                            </ul>
                        </div>
                        
                        <div class="bg-blue-800 p-4 rounded-lg">
                            <h4 class="font-semibold border-b border-blue-600 pb-2 mb-2">日間高峰時段 (14:00-16:00)</h4>
                            <ul class="space-y-1">
                                <li>水溫升至29.2℃</li>
                                <li>遊客密度激增至每100平方米80人</li>
                                <li>大腸菌群含量也隨之上升至150 CFU/100ml</li>
                            </ul>
                        </div>
                        
                        <div class="bg-blue-800 p-4 rounded-lg">
                            <h4 class="font-semibold border-b border-blue-600 pb-2 mb-2">黃昏時段 (17:30-18:10)</h4>
                            <ul class="space-y-1">
                                <li>各項指標趨於平穩</li>
                                <li>水溫26.9℃</li>
                                <li>遊客密度降至40人/100㎡</li>
                            </ul>
                        </div>
                    </div>
                    
                    <h4 class="font-semibold mb-3">季節變化：</h4>
                    <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
                        <div class="bg-blue-800 p-3 rounded-lg">
                            <h5 class="font-medium border-b border-blue-600 pb-1 mb-2">春季</h5>
                            <ul class="text-sm">
                                <li>水溫: 22-25℃</li>
                                <li>鹽度: 比年平均高0.2%</li>
                                <li>特點: 藻類開始繁殖</li>
                            </ul>
                        </div>
                        
                        <div class="bg-blue-800 p-3 rounded-lg">
                            <h5 class="font-medium border-b border-blue-600 pb-1 mb-2">夏季</h5>
                            <ul class="text-sm">
                                <li>水溫: 28-31℃</li>
                                <li>鹽度: 下降0.5%</li>
                                <li>特點: 開始出現水母</li>
                            </ul>
                        </div>
                        
                        <div class="bg-blue-800 p-3 rounded-lg">
                            <h5 class="font-medium border-b border-blue-600 pb-1 mb-2">秋季</h5>
                            <ul class="text-sm">
                                <li>水溫: 25-28℃</li>
                                <li>鹽度: 回升0.3%</li>
                                <li>特點: 最適宜遊覽的季節</li>
                            </ul>
                        </div>
                        
                        <div class="bg-blue-800 p-3 rounded-lg">
                            <h5 class="font-medium border-b border-blue-600 pb-1 mb-2">冬季</h5>
                            <ul class="text-sm">
                                <li>水溫: 18-22℃</li>
                                <li>鹽度: 上升0.8%</li>
                                <li>特點: 風浪較為明顯</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="bg-yellow-50 border-l-4 border-yellow-400 p-5 rounded-lg">
                    <h3 class="text-lg font-semibold text-yellow-800 mb-3">重要發現</h3>
                    <p class="mb-3">檢測數據中，電導率達到18.65ms/cm，這一數值是內港水域（1.38ms/cm）的13.5倍，表明黑沙海灘具有典型的半封閉海灣特徵。鹽度1.67%的測量值也顯著高於周邊海域平均水平，可能與有限的海水交換有關。</p>
                    <p class="mb-3">特別值得注意的是，總溶解固體（TDS）的檢測值存在單位混淆的情況，需要進一步複核確認。</p>
                    <p>在安全評估方面，所有生物指標均符合游泳安全標準。其中大腸菌群含量85 CFU/100ml，遠低於200 CFU/100ml的安全限值。夏季午後水溫可能接近31℃的上限，遊客需注意防暑。退潮時部分區域礁石裸露，需要特別小心。</p>
                </div>
            </section>
            
            <!-- 環境思考 -->
            <section id="content3" class="tab-content bg-white rounded-lg shadow-md p-6 mb-8">
                <h2 class="text-2xl font-bold text-blue-800 mb-6">澳門海域水環境的思考</h2>
                
                <div class="mb-8">
                    <h3 class="text-xl font-semibold text-blue-700 mb-4">分享您的環境思考</h3>
                    <p class="mb-4">請在下方輸入您對澳門海域水環境的看法、觀察或建議。您的想法將會顯示在下方的「環境思考區」。</p>
                    
                    <div class="mb-4">
                        <label for="thoughtName" class="block text-sm font-medium text-gray-700 mb-1">您的姓名</label>
                        <input type="text" id="thoughtName" class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" placeholder="輸入您的姓名（可選）">
                    </div>
                    
                    <div class="mb-4">
                        <label for="thoughtTitle" class="block text-sm font-medium text-gray-700 mb-1">標題</label>
                        <input type="text" id="thoughtTitle" class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" placeholder="輸入您的思考標題">
                    </div>
                    
                    <div class="mb-4">
                        <label for="thoughtContent" class="block text-sm font-medium text-gray-700 mb-1">內容</label>
                        <textarea id="thoughtContent" rows="6" class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" placeholder="分享您對澳門海域水環境的看法..."></textarea>
                    </div>
                    
                    <button id="addThought" class="bg-blue-600 text-white px-4 py-2 rounded-lg font-medium hover:bg-blue-700 transition duration-300">添加我的思考</button>
                </div>
                
                <div class="mb-8">
                    <h3 class="text-xl font-semibold text-blue-700 mb-4">環境思考區</h3>
                    <div id="thoughtsContainer" class="space-y-4">
                        <!-- 預設思考內容 -->
                        <div class="thought-card">
                            <div class="flex justify-between items-center mb-2">
                                <h4 class="text-lg font-semibold text-blue-800">海灘垃圾問題亟待解決</h4>
                                <span class="text-sm text-gray-500">黃教授 | 2025/05/27 09:15</span>
                            </div>
                            <p>在最近一次黑沙海灘調查中，我發現岸邊塑料垃圾數量明顯增加。建議增設分類垃圾桶，並定期組織志願者清理活動。同時，應加強環保宣傳，提高遊客的環保意識。</p>
                        </div>
                        
                        <div class="thought-card">
                            <div class="flex justify-between items-center mb-2">
                                <h4 class="text-lg font-semibold text-blue-800">關於電導率異常的思考</h4>
                                <span class="text-sm text-gray-500">陳研究員 | 2025/05/26 16:30</span>
                            </div>
                            <p>黑沙海灘電導率高達18.65ms/cm，遠高於內港水域，這可能與海灘特殊的地質結構有關。建議進行更深入的地質調查，分析海綠石礦物對水質的影響。同時，應建立長期監測站點，追蹤電導率的季節性變化。</p>
                        </div>
                    </div>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
                    <div>
                        <h3 class="text-xl font-semibold text-blue-700 mb-4">黑沙海灘的獨特性</h3>
                        <div class="bg-blue-50 p-5 rounded-lg">
                            <p class="mb-4">通過對比黑沙海灘與內港水域的數據，我們發現黑沙海灘具有非常獨特的水質特徵。特別是電導率和鹽度的顯著差異，表明這兩個水域的水體交換和循環機制存在本質區別。</p>
                            <p>黑沙海灘作為半封閉海灣，其水質受到周邊地質環境和海洋動力學的雙重影響。海綠石礦物的存在不僅賦予了沙灘獨特的黑色外觀，也可能對水體的化學特性產生影響。</p>
                        </div>
                        
                        <h3 class="text-xl font-semibold text-blue-700 mt-6 mb-4">人類活動的影響</h3>
                        <div class="bg-blue-50 p-5 rounded-lg">
                            <p class="mb-4">我們的研究發現，遊客活動與水質指標之間存在明顯的相關性。在遊客密度高峰期（每100平方米80人），大腸菌群含量上升至150 CFU/100ml，雖然仍在安全範圍內，但比清晨時段高出近一倍。</p>
                            <p>岸邊散落的塑料垃圾不僅影響景觀，長期來看也可能對海洋生態系統造成威脅。我們建議加強環境教育和垃圾管理，減少人類活動對這一珍貴自然資源的負面影響。</p>
                        </div>
                    </div>
                    
                    <div>
                        <h3 class="text-xl font-semibold text-blue-700 mb-4">水質與生態健康</h3>
                        <div class="bg-blue-50 p-5 rounded-lg">
                            <p class="mb-4">黑沙海灘的葉綠素a含量（2.1μg/L）比內港低40%，表明水體中藻類生物量處於健康水平，不存在富營養化問題。這與海灘開闊的地理位置和良好的水體交換能力有關。</p>
                            <p>透明度指標（平均1.3m）也顯著高於內港（0.8m），進一步證實了黑沙海灘水質的優越性。這為海洋生物提供了良好的生存環境，也為遊客創造了更佳的遊覽體驗。</p>
                        </div>
                        
                        <h3 class="text-xl font-semibold text-blue-700 mt-6 mb-4">未來挑戰與建議</h3>
                        <div class="bg-blue-50 p-5 rounded-lg">
                            <p class="mb-4">面對氣候變化和城市化的雙重壓力，澳門海域水環境面臨諸多挑戰。我們建議：</p>
                            <ul class="list-disc pl-5 space-y-2">
                                <li>建立長期監測網絡，定期發布水質報告</li>
                                <li>制定科學的遊客容量管理策略，避免過度使用</li>
                                <li>加強海灘周邊的垃圾收集和分類處理</li>
                                <li>開展海洋環保教育，提高公眾意識</li>
                                <li>研究氣候變化對海灘生態系統的潛在影響</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="bg-blue-700 text-white p-6 rounded-lg">
                    <h3 class="text-xl font-bold mb-4">綜合評估與展望</h3>
                    <p class="mb-4">綜合各項指標，黑沙海灘的水質狀況總體良好，適合開展水上娛樂活動。特別是在衛生指標方面，大腸菌群含量遠低於安全限值，表明水體微生物污染風險低。</p>
                    <p class="mb-4">然而，我們也注意到一些需要關注的問題：</p>
                    <ol class="list-decimal pl-5 space-y-2 mb-4">
                        <li>電導率異常高的原因尚未完全明確，需要進一步研究</li>
                        <li>岸邊垃圾問題需要系統性解決方案</li>
                        <li>遊客高峰期的水質管理需要加強</li>
                    </ol>
                    <p>作為澳門最具特色的自然景觀之一，黑沙海灘的保護和可持續利用需要政府、研究機構和公眾的共同努力。我們期待通過持續的監測和研究，為澳門海域水環境的改善提供科學依據。</p>
                </div>
            </section>
            
            <!-- 團隊與聲明 -->
            <section id="content4" class="tab-content bg-white rounded-lg shadow-md p-6">
                <h2 class="text-2xl font-bold text-blue-800 mb-6">團隊分工與聲明</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
                    <div>
                        <h3 class="text-xl font-semibold text-blue-700 mb-4">檢測團隊分工</h3>
                        <div class="table-container">
                            <table class="w-full">
                                <thead>
                                    <tr>
                                        <th>項目與參與者</th>
                                        <th>人員名單</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>取水員</td>
                                        <td>黃梓鋒、殷頌熙</td>
                                    </tr>
                                    <tr>
                                        <td>檢測員</td>
                                        <td>二谷遙希、陳梓鍵</td>
                                    </tr>
                                    <tr>
                                        <td>記錄員</td>
                                        <td>二谷遙希、黃梓鋒</td>
                                    </tr>
                                    <tr>
                                        <td>拍攝員</td>
                                        <td>廖俊榮、陳梓鍵</td>
                                    </tr>
                                    <tr>
                                        <td>其他參與人員</td>
                                        <td>陳梓鍵、黃梓鋒、殷頌熙、二谷遙希、廖俊榮</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        
                        <div class="mt-8">
                            <h3 class="text-xl font-semibold text-blue-700 mb-4">團隊成員介紹</h3>
                            <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
                                <div class="bg-blue-50 p-4 rounded-lg">
                                    <div class="flex items-center justify-center mb-3">
                                        <svg class="w-16 h-16 text-blue-700" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path>
                                        </svg>
                                    </div>
                                    <h4 class="font-medium text-center">陳梓鍵</h4>
                                    <p class="text-sm text-center text-gray-600">檢測員、拍攝員</p>
                                </div>
                                
                                <div class="bg-blue-50 p-4 rounded-lg">
                                    <div class="flex items-center justify-center mb-3">
                                        <svg class="w-16 h-16 text-blue-700" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path>
                                        </svg>
                                    </div>
                                    <h4 class="font-medium text-center">黃梓鋒</h4>
                                    <p class="text-sm text-center text-gray-600">取水員、記錄員</p>
                                </div>
                                
                                <div class="bg-blue-50 p-4 rounded-lg">
                                    <div class="flex items-center justify-center mb-3">
                                        <svg class="w-16 h-16 text-blue-700" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path>
                                        </svg>
                                    </div>
                                    <h4 class="font-medium text-center">殷頌熙</h4>
                                    <p class="text-sm text-center text-gray-600">取水員</p>
                                </div>
                                
                                <div class="bg-blue-50 p-4 rounded-lg">
                                    <div class="flex items-center justify-center mb-3">
                                        <svg class="w-16 h-16 text-blue-700" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path>
                                        </svg>
                                    </div>
                                    <h4 class="font-medium text-center">二谷遙希</h4>
                                    <p class="text-sm text-center text-gray-600">檢測員、記錄員</p>
                                </div>
                                
                                <div class="bg-blue-50 p-4 rounded-lg">
                                    <div class="flex items-center justify-center mb-3">
                                        <svg class="w-16 h-16 text-blue-700" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"></path>
                                        </svg>
                                    </div>
                                    <h4 class="font-medium text-center">廖俊榮</h4>
                                    <p class="text-sm text-center text-gray-600">拍攝員</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div>
                        <h3 class="text-xl font-semibold text-blue-700 mb-4">檢測聲明</h3>
                        <div class="bg-blue-50 p-5 rounded-lg mb-6">
                            <p class="mb-4">本報告由澳門環保志工協會檢測團隊於2025年5月26日完成，所有數據真實可靠。</p>
                            <p class="font-medium mb-2">完整原始記錄包含：</p>
                            <ul class="list-disc pl-5 space-y-2">
                                <li>現場檢測視頻（由廖俊榮、陳梓鍵拍攝）</li>
                                <li>原始記錄表（二谷遙希、黃梓鋒記錄）</li>
                                <li>水樣標本（黃梓鋒、殷頌熙採集）</li>
                            </ul>
                        </div>
                        
                        <h3 class="text-xl font-semibold text-blue-700 mb-4">研究方法與標準</h3>
                        <div class="bg-blue-50 p-5 rounded-lg">
                            <p class="mb-4">本研究嚴格遵循國際水質監測標準和規範，採用科學的採樣和分析方法，確保數據的準確性和可靠性。</p>
                            <p class="mb-4">水質評價參考標準：</p>
                            <ul class="list-disc pl-5 space-y-2">
                                <li>《海水水質標準》(GB 3097-1997)</li>
                                <li>《澳門特別行政區海域水質標準》</li>
                                <li>世界衛生組織(WHO)休閒用水指南</li>
                            </ul>
                        </div>
                        
                        <div class="mt-6 bg-blue-700 text-white p-5 rounded-lg">
                            <h3 class="text-lg font-bold mb-3">聯絡資訊</h3>
                            <p class="mb-2">如對本報告有任何疑問或建議，請聯絡：</p>
                            <p class="mb-1">澳門環保志工協會</p>
                            <p class="mb-1">電郵：info@macaueco.org</p>
                            <p>電話：+853 XXXX XXXX</p>
                        </div>
                    </div>
                </div>
                
                <div class="border-t border-gray-200 pt-6 mt-6">
                    <p class="text-center text-gray-600">© 2025 澳門環保志工協會 - 黑沙海灘水質研究項目</p>
                    <p class="text-center text-gray-500 text-sm mt-2">本報告僅供環境教育和研究參考，未經許可不得用於商業用途</p>
                </div>
            </section>
        </main>
    </div>
    
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const tabBtns = document.querySelectorAll('.tab-btn');
            const tabContents = document.querySelectorAll('.tab-content');
            
            // 初始化本地存儲
            if (!localStorage.getItem('environmentalThoughts')) {
                // 預設思考內容
                const defaultThoughts = [
                    {
                        name: '黃教授',
                        title: '海灘垃圾問題亟待解決',
                        content: '在最近一次黑沙海灘調查中，我發現岸邊塑料垃圾數量明顯增加。建議增設分類垃圾桶，並定期組織志願者清理活動。同時，應加強環保宣傳，提高遊客的環保意識。',
                        date: '2025/05/27 09:15'
                    },
                    {
                        name: '陳研究員',
                        title: '關於電導率異常的思考',
                        content: '黑沙海灘電導率高達18.65ms/cm，遠高於內港水域，這可能與海灘特殊的地質結構有關。建議進行更深入的地質調查，分析海綠石礦物對水質的影響。同時，應建立長期監測站點，追蹤電導率的季節性變化。',
                        date: '2025/05/26 16:30'
                    }
                ];
                localStorage.setItem('environmentalThoughts', JSON.stringify(defaultThoughts));
            }
            
            // 載入思考內容
            loadThoughts();
            
            tabBtns.forEach(btn => {
                btn.addEventListener('click', () => {
                    const tabId = btn.id;
                    const contentId = 'content' + tabId.substring(3);
                    
                    // Update button styles
                    tabBtns.forEach(b => {
                        b.classList.remove('bg-blue-600', 'text-white');
                        b.classList.add('bg-blue-100', 'text-blue-800');
                    });
                    btn.classList.remove('bg-blue-100', 'text-blue-800');
                    btn.classList.add('bg-blue-600', 'text-white');
                    
                    // Show selected content
                    tabContents.forEach(content => {
                        content.classList.remove('active');
                    });
                    document.getElementById(contentId).classList.add('active');
                });
            });
            
            // Handle adding thoughts
            const addThoughtBtn = document.getElementById('addThought');
            
            addThoughtBtn.addEventListener('click', () => {
                const name = document.getElementById('thoughtName').value.trim() || '匿名用戶';
                const title = document.getElementById('thoughtTitle').value.trim();
                const content = document.getElementById('thoughtContent').value.trim();
                
                if (title === '' || content === '') {
                    alert('請輸入標題和內容');
                    return;
                }
                
                // 獲取當前日期和時間
                const now = new Date();
                const dateStr = `${now.getFullYear()}/${String(now.getMonth()+1).padStart(2, '0')}/${String(now.getDate()).padStart(2, '0')} ${String(now.getHours()).padStart(2, '0')}:${String(now.getMinutes()).padStart(2, '0')}`;
                
                // 創建新思考
                const newThought = {
                    name: name,
                    title: title,
                    content: content,
                    date: dateStr
                };
                
                // 保存到本地存儲
                const thoughts = JSON.parse(localStorage.getItem('environmentalThoughts'));
                thoughts.unshift(newThought); // 添加到數組開頭
                localStorage.setItem('environmentalThoughts', JSON.stringify(thoughts));
                
                // 重新載入思考內容
                loadThoughts();
                
                // 清空輸入欄位
                document.getElementById('thoughtName').value = '';
                document.getElementById('thoughtTitle').value = '';
                document.getElementById('thoughtContent').value = '';
                
                // 顯示成功消息
                alert('您的環境思考已成功添加！');
            });
            
            // 載入思考內容的函數
            function loadThoughts() {
                const thoughtsContainer = document.getElementById('thoughtsContainer');
                const thoughts = JSON.parse(localStorage.getItem('environmentalThoughts'));
                
                // 清空容器
                thoughtsContainer.innerHTML = '';
                
                if (thoughts.length === 0) {
                    thoughtsContainer.innerHTML = `
                        <div class="bg-gray-100 p-6 rounded-lg text-center text-gray-500">
                            <p>暫無環境思考，請添加您的想法</p>
                        </div>
                    `;
                    return;
                }
                
                // 添加所有思考
                thoughts.forEach(thought => {
                    const thoughtCard = document.createElement('div');
                    thoughtCard.className = 'thought-card';
                    
                    thoughtCard.innerHTML = `
                        <div class="flex justify-between items-center mb-2">
                            <h4 class="text-lg font-semibold text-blue-800">${thought.title}</h4>
                            <span class="text-sm text-gray-500">${thought.name} | ${thought.date}</span>
                        </div>
                        <p>${thought.content}</p>
                    `;
                    
                    thoughtsContainer.appendChild(thoughtCard);
                });
            }
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'94f7c97f21cb7c5e',t:'MTc0OTg4MjcxMS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
