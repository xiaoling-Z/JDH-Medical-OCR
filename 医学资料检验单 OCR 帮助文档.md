# 医学资料检验单 OCR 帮助文档
## 接口说明
该API用于对拍照上传的各类医学检验资料（检验单、报告单等）进行识别和专业的医学解析
## 请求URl
POST /extract/inspection/v1
#### 请求体字段数据结构说明
| 参数名称 | 参数类型 | 是否必须 | 描述 | 示例值 |
|-------|-------|-------|-------|-------|
| image_url | String | 是 | 待解析图片url地址链接 | https://image.healthjd.com/nethpimage/jfs/t1/200642/2/43118/95355/665eae8bF8b735b6b/fc176e43b7802a50.jpg |
#### 请求头参数
| 参数名称 | 参数值 | 
|-------|-------|
| Content-Type | application/json | 
## 请求响应示例
```
Headers:
Content-Type: application/json

Body:
{
"url":"https://image.healthjd.com/nethpimage/jfs/t1/200642/2/43118/95355/665eae8bF8b735b6b/fc176e43b7802a50.jpg"
}

```
```
HTTP/1.1 200 OK

{
    "code": 0,
    "data": {
        "info": {
            "age": "12岁",
            "department": "儿内科一门诊",
            "gender": "男",
            "iDcard": null,
            "name": "李泽昊",
            "organization": "哈尔滨医科大学附属第二医院",
            "phone": null,
            "reportCode": null,
            "reportName": "检验报告单",
            "time": null
        },
        "table": {
            "data": [
                {
                    "abbreviation": "WBC",
                    "diagnose": "0",
                    "entryname": "白细胞计数",
                    "entrynameCode": "D040010010001",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            39.0710563659668,
                            197.2966766357422
                        ],
                        [
                            743.0655517578125,
                            193.05177307128906
                        ],
                        [
                            743.1035766601562,
                            215.70404052734375
                        ],
                        [
                            39.106895446777344,
                            218.64598083496094
                        ]
                    ],
                    "reference": {
                        "max": "11.3",
                        "min": "4.3",
                        "ref": "4.3-11.3"
                    },
                    "result": "9.8",
                    "unit": "10/L"
                },
                {
                    "abbreviation": "NEUT%",
                    "diagnose": "0",
                    "entryname": "中性粒细胞百分率",
                    "entrynameCode": "D040010010032",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            40.0972900390625,
                            217.12135314941406
                        ],
                        [
                            745.094970703125,
                            215.05743408203125
                        ],
                        [
                            745.1317138671875,
                            236.70135498046875
                        ],
                        [
                            40.13379669189453,
                            238.69168090820312
                        ]
                    ],
                    "reference": {
                        "max": "70.0",
                        "min": "31.0",
                        "ref": "31.0-70.0"
                    },
                    "result": "49.8",
                    "unit": "%"
                },
                {
                    "abbreviation": "LYM%",
                    "diagnose": "0",
                    "entryname": "淋巴细胞百分率",
                    "entrynameCode": "D040010010017",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            37.12874221801758,
                            238.12701416015625
                        ],
                        [
                            746.1270141601562,
                            235.68475341796875
                        ],
                        [
                            746.1624145507812,
                            259.70001220703125
                        ],
                        [
                            38.16456604003906,
                            261.69268798828125
                        ]
                    ],
                    "reference": {
                        "max": "59.0",
                        "min": "23.0",
                        "ref": "23.0-59.0"
                    },
                    "result": "36.1",
                    "unit": "%"
                },
                {
                    "abbreviation": "MONO%",
                    "diagnose": "2",
                    "entryname": "单核细胞百分数",
                    "entrynameCode": "D040010010038",
                    "methodology": "流式+电阻抗",
                    "notes": 2,
                    "points": [
                        [
                            37.1568489074707,
                            259.13037109375
                        ],
                        [
                            746.1517333984375,
                            256.6847229003906
                        ],
                        [
                            746.1865844726562,
                            277.6999816894531
                        ],
                        [
                            38.192527770996094,
                            282.6472473144531
                        ]
                    ],
                    "reference": {
                        "max": "8.0",
                        "min": "3.0",
                        "ref": "3.0-8.0"
                    },
                    "result": "10.2",
                    "unit": "%"
                },
                {
                    "abbreviation": "EO%",
                    "diagnose": "0",
                    "entryname": "嗜酸性粒细胞百分率",
                    "entrynameCode": "D040010010015",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            36.18913650512695,
                            280.9677429199219
                        ],
                        [
                            749.1802978515625,
                            276.7258605957031
                        ],
                        [
                            749.2173461914062,
                            300.6959533691406
                        ],
                        [
                            36.219451904296875,
                            302.70367431640625
                        ]
                    ],
                    "reference": {
                        "max": "9.0",
                        "min": "0.0",
                        "ref": "0.0-9.0"
                    },
                    "result": "3.5",
                    "unit": "%"
                },
                {
                    "abbreviation": "BASO%",
                    "diagnose": "0",
                    "entryname": "嗜碱性粒细胞百分率",
                    "entrynameCode": "D040010010016",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            36.2157096862793,
                            301.4611511230469
                        ],
                        [
                            749.2067260742188,
                            297.725830078125
                        ],
                        [
                            749.2449951171875,
                            319.89642333984375
                        ],
                        [
                            36.24738693237305,
                            323.64990234375
                        ]
                    ],
                    "reference": {
                        "max": "1",
                        "min": "0",
                        "ref": "0-1"
                    },
                    "result": "0.4",
                    "unit": "%"
                },
                {
                    "abbreviation": "NEUT",
                    "diagnose": "0",
                    "entryname": "中性粒细胞绝对值",
                    "entrynameCode": "D040010010012",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            37.241676330566406,
                            322.3075866699219
                        ],
                        [
                            752.2426147460938,
                            320.2202453613281
                        ],
                        [
                            752.2721557617188,
                            341.6918640136719
                        ],
                        [
                            37.2759895324707,
                            343.70562744140625
                        ]
                    ],
                    "reference": {
                        "max": "7.8",
                        "min": "1.6",
                        "ref": "1.6-7.8"
                    },
                    "result": "4.90",
                    "unit": "10°/L"
                },
                {
                    "abbreviation": "LYM",
                    "diagnose": "0",
                    "entryname": "淋巴细胞绝对值",
                    "entrynameCode": "D040010010010",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            37.25859832763672,
                            340.70733642578125
                        ],
                        [
                            754.270751953125,
                            341.2158508300781
                        ],
                        [
                            753.3015747070312,
                            363.6905517578125
                        ],
                        [
                            37.30224609375,
                            364.6485290527344
                        ]
                    ],
                    "reference": {
                        "max": "4.6",
                        "min": "1.5",
                        "ref": "1.5-4.6"
                    },
                    "result": "3.60",
                    "unit": "10/L"
                },
                {
                    "abbreviation": "MON",
                    "diagnose": "2",
                    "entryname": "单核细胞检测值",
                    "entrynameCode": "D040010010021",
                    "methodology": "流式+电阻抗",
                    "notes": 2,
                    "points": [
                        [
                            36.29908752441406,
                            364.71197509765625
                        ],
                        [
                            754.3002319335938,
                            362.6891784667969
                        ],
                        [
                            754.334228515625,
                            385.61700439453125
                        ],
                        [
                            36.33301544189453,
                            387.6498107910156
                        ]
                    ],
                    "reference": {
                        "max": "0.76",
                        "min": "0.13",
                        "ref": "0.13-0.76"
                    },
                    "result": "1.00",
                    "unit": "10/L"
                },
                {
                    "abbreviation": "EO",
                    "diagnose": "0",
                    "entryname": "嗜酸性粒细胞值",
                    "entrynameCode": "D040010010055",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            36.32698059082031,
                            387.31219482421875
                        ],
                        [
                            755.32958984375,
                            385.21282958984375
                        ],
                        [
                            755.3662719726562,
                            406.8548278808594
                        ],
                        [
                            36.363746643066406,
                            408.96759033203125
                        ]
                    ],
                    "reference": {
                        "max": "0.68",
                        "min": "0.00",
                        "ref": "0.00-0.68"
                    },
                    "result": "0.30",
                    "unit": "10/L"
                },
                {
                    "abbreviation": "BASO",
                    "diagnose": "0",
                    "entryname": "嗜碱性粒细胞值",
                    "entrynameCode": "D040010010057",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            36.35329055786133,
                            407.71697998046875
                        ],
                        [
                            757.3577880859375,
                            405.6851501464844
                        ],
                        [
                            757.3924560546875,
                            428.8722229003906
                        ],
                        [
                            36.39486312866211,
                            430.970947265625
                        ]
                    ],
                    "reference": {
                        "max": "0.07",
                        "min": "0.00",
                        "ref": "0.00-0.07"
                    },
                    "result": "0.00",
                    "unit": "10/L"
                },
                {
                    "abbreviation": "HGB",
                    "diagnose": "0",
                    "entryname": "血红蛋白",
                    "entrynameCode": "D040010010003",
                    "methodology": "SLS比色法",
                    "notes": 0,
                    "points": [
                        [
                            34.386417388916016,
                            428.72296142578125
                        ],
                        [
                            745.3859252929688,
                            426.701171875
                        ],
                        [
                            745.4259643554688,
                            451.677490234375
                        ],
                        [
                            33.42012023925781,
                            452.1421813964844
                        ]
                    ],
                    "reference": {
                        "max": "160",
                        "min": "110",
                        "ref": "110-160"
                    },
                    "result": "142",
                    "unit": "g/L"
                },
                {
                    "abbreviation": "RBC",
                    "diagnose": "0",
                    "entryname": "红细胞计数",
                    "entrynameCode": "D040010010002",
                    "methodology": "电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            36.413841247558594,
                            451.72027587890625
                        ],
                        [
                            722.4166870117188,
                            449.7319641113281
                        ],
                        [
                            722.4534912109375,
                            471.9541320800781
                        ],
                        [
                            36.450721740722656,
                            473.97088623046875
                        ]
                    ],
                    "reference": {
                        "max": "5.70",
                        "min": "4.20",
                        "ref": "4.20-5.70"
                    },
                    "result": "4.98",
                    "unit": "10/L"
                },
                {
                    "abbreviation": "PCV",
                    "diagnose": "0",
                    "entryname": "血细胞比容测定",
                    "entrynameCode": "D040010010035",
                    "methodology": "电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            35.44754409790039,
                            473.47235107421875
                        ],
                        [
                            723.4453125,
                            471.4729919433594
                        ],
                        [
                            723.480712890625,
                            493.76544189453125
                        ],
                        [
                            35.48048782348633,
                            494.97052001953125
                        ]
                    ],
                    "reference": {
                        "max": "50",
                        "min": "37",
                        "ref": "37-50"
                    },
                    "result": "43.2",
                    "unit": "%"
                },
                {
                    "abbreviation": "RBC",
                    "diagnose": "0",
                    "entryname": "红细胞计数",
                    "entrynameCode": "D040010010002",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            37.47529602050781,
                            495.4663391113281
                        ],
                        [
                            599.4756469726562,
                            493.8964538574219
                        ],
                        [
                            599.5125122070312,
                            516.1270141601562
                        ],
                        [
                            36.50991439819336,
                            516.967529296875
                        ]
                    ],
                    "reference": {
                        "max": "92.0",
                        "min": "77.0",
                        "ref": "77.0-92.0"
                    },
                    "result": "86.9",
                    "unit": "fl"
                },
                {
                    "abbreviation": "MCH",
                    "diagnose": "0",
                    "entryname": "平均红细胞血红蛋白量",
                    "entrynameCode": "D040010010008",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            37.504398345947266,
                            518.46630859375
                        ],
                        [
                            599.5064697265625,
                            516.8964233398438
                        ],
                        [
                            599.5404663085938,
                            537.6505126953125
                        ],
                        [
                            37.53871154785156,
                            539.3090209960938
                        ]
                    ],
                    "reference": {
                        "max": "34.0",
                        "min": "25.0",
                        "ref": "25.0-34.0"
                    },
                    "result": "28.5",
                    "unit": "pg"
                },
                {
                    "abbreviation": "MCHC",
                    "diagnose": "0",
                    "entryname": "平均红细胞血红蛋白浓度",
                    "entrynameCode": "D040010010009",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            36.53083801269531,
                            539.47265625
                        ],
                        [
                            584.5345458984375,
                            537.9164428710938
                        ],
                        [
                            584.568359375,
                            559.708984375
                        ],
                        [
                            36.56648254394531,
                            561.31201171875
                        ]
                    ],
                    "reference": {
                        "max": "355",
                        "min": "310",
                        "ref": "310-355"
                    },
                    "result": "328",
                    "unit": "g/L"
                },
                {
                    "abbreviation": "RDW-CV",
                    "diagnose": "0",
                    "entryname": "红细胞分布宽度",
                    "entrynameCode": "",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            35.56614685058594,
                            562.3133544921875
                        ],
                        [
                            599.5645751953125,
                            560.6421508789062
                        ],
                        [
                            599.6009521484375,
                            582.1771850585938
                        ],
                        [
                            35.59526062011719,
                            583.6510009765625
                        ]
                    ],
                    "reference": {
                        "max": "14.5",
                        "min": "11.5",
                        "ref": "11.5-14.5"
                    },
                    "result": "13.2",
                    "unit": "%"
                },
                {
                    "abbreviation": "RDW-SD",
                    "diagnose": "3",
                    "entryname": "红细胞分布宽度",
                    "entrynameCode": "",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            36.591697692871094,
                            584.133056640625
                        ],
                        [
                            452.59442138671875,
                            582.9442138671875
                        ],
                        [
                            452.6241149902344,
                            602.8003540039062
                        ],
                        [
                            36.62298583984375,
                            603.9707641601562
                        ]
                    ],
                    "reference": {
                        "max": null,
                        "min": null,
                        "ref": null
                    },
                    "result": "39.4",
                    "unit": "fl"
                },
                {
                    "abbreviation": "PLT",
                    "diagnose": "0",
                    "entryname": "血小板计数",
                    "entrynameCode": "D040010010004",
                    "methodology": "流式+电阻抗",
                    "notes": 0,
                    "points": [
                        [
                            35.61722946166992,
                            603.7265014648438
                        ],
                        [
                            761.61865234375,
                            600.6795654296875
                        ],
                        [
                            761.6569213867188,
                            625.607421875
                        ],
                        [
                            35.65412902832031,
                            627.6509399414062
                        ]
                    ],
                    "reference": {
                        "max": "407",
                        "min": "150",
                        "ref": "150-407"
                    },
                    "result": "353",
                    "unit": "10^9/L"
                },
                {
                    "abbreviation": "MPV",
                    "diagnose": "1",
                    "entryname": "血小板平均体积",
                    "entrynameCode": "D040010010011",
                    "methodology": "",
                    "notes": 1,
                    "points": [
                        [
                            35.65193176269531,
                            627.4755859375
                        ],
                        [
                            595.6522827148438,
                            625.9016723632812
                        ],
                        [
                            595.6871337890625,
                            649.1406860351562
                        ],
                        [
                            35.68490219116211,
                            650.6509399414062
                        ]
                    ],
                    "reference": {
                        "max": "11.0",
                        "min": "7.0",
                        "ref": "7.0-11.0"
                    },
                    "result": "6.7",
                    "unit": "f1"
                },
                {
                    "abbreviation": "PDW",
                    "diagnose": "0",
                    "entryname": "血小板分布宽度",
                    "entrynameCode": "D040010010036",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            36.682518005371094,
                            650.9674682617188
                        ],
                        [
                            600.6810302734375,
                            649.319580078125
                        ],
                        [
                            600.7133178710938,
                            669.49853515625
                        ],
                        [
                            36.7131233215332,
                            671.1346435546875
                        ]
                    ],
                    "reference": {
                        "max": "17.0",
                        "min": "15.0",
                        "ref": "15.0-17.0"
                    },
                    "result": "16.1",
                    "unit": "%"
                },
                {
                    "abbreviation": "PCT",
                    "diagnose": "0",
                    "entryname": "血小板压积",
                    "entrynameCode": "D040010010037",
                    "methodology": "",
                    "notes": 0,
                    "points": [
                        [
                            33.711978912353516,
                            672.9797973632812
                        ],
                        [
                            614.7052612304688,
                            669.0349731445312
                        ],
                        [
                            614.744384765625,
                            692.0365600585938
                        ],
                        [
                            34.746456146240234,
                            696.6522827148438
                        ]
                    ],
                    "reference": {
                        "max": "0.282",
                        "min": "0.108",
                        "ref": "0.108-0.282"
                    },
                    "result": "0.236",
                    "unit": "%"
                }
            ],
            "title": "",
            "type": "血常规"
        }
    }
}
```
