서브스텐스 디자이너

- 비용
  - 스팀 15만원정도함 년마다 나오니 1월에 이전버전 세일 노리는것도
  - 학생용은 1년마다 갱신하는 방식

- [udemy: The Ultimate 2D & 3D Shader Graph VFX Unity Course](https://www.udemy.com/course/the-ultimate-2d-3d-shader-graph-vfx-unity-course/)
- [[나만의 게임 텍스처 제작] 서브스탠스 디자이너의 모든 것](https://www.inflearn.com/course/게임텍스처-섭스턴스-디자이너/)

- https://helpx.adobe.com/substance-3d-designer/home.html
  - https://helpx.adobe.com/substance-3d-designer/getting-started/tutorials-learning.html
- [Substance 3D Designer Quick Tips | Adobe Substance 3D](https://www.youtube.com/playlist?list=PLB0wXHrWAmCy457vxKM4rQuJ-nvYm9j4M) 


- [1MaxFX -  Textures Tutorial](https://www.youtube.com/playlist?list=PLRpiOeaDPL_6t0WEUgaxrekJG5ocxW-lX)


https://www.artstation.com/learning/adobe-substance-3d-designer
https://www.artstation.com/learning/courses/PJo/intro-to-substance-designer-for-vfx/
  Bruno Afonseca
  https://3dbruno.com/


https://www.artstation.com/learning/courses/PJo/intro-to-substance-designer-for-vfx/chapters/Wnp8/sd-nodes-flowmaps-vector-warp-channels-shuffle
  노말로 별을 휘게 만들기

이주영
https://coloso.co.kr/products/gamegraphic_yijuyeong
[2019 - [NDC] 섭스턴스 디자이너 고급 테크닉 - FX맵을 사용한 규칙적인 패턴 배치](https://youtu.be/t1D9Wr2YEWs?si=gUc-kETOpEGHcsgI)
[2019 - [NDC] Substance Painter + Designer beyond Materials](https://youtu.be/8ewBNG3KTik?si=AuVeDcN07DnbDEXM)


- [free - Substance Player](https://helpx.adobe.com/substance-3d-player/home.html)
  - Drag and drop Substance 3D files (SBSAR or SBS) into the application, adjust the content with easy-to-use parameter widgets and see instant variations in 2D and 3D views simultaneously.



SBS files are editable and can be opened in Substance Designer or Substance Alchemist.
SBSAR stands for Substance Archive, and it contains a compressed version of your material, with only the exposed parameters and outputs

- 파라미터 설정법
  - https://helpx.adobe.com/substance-3d-designer/using/exposing-parameters.html
  - https://helpx.adobe.com/substance-3d-designer/substance-model-graphs/exposing-parameters.html
  - 그룹핑
  - 파라미터 설정값에 의한 비지블 설정
    - https://helpx.adobe.com/substance-3d-designer/substance-compositing-graphs/exposing-a-parameter/visible-if-control-visibility-of-inputs-outputs-and-parameters.html
    - input["A"]==true

## 초기

- 템플릿 폴더 설정: Preference > Projects > Project > General 탭
  - https://youtu.be/SAMyIxp0Le8?si=fQLVwGUNpjLr7Tdr
- 라이브러리 폴더 설정: Preference > Projects > Project > Library 탭

## 키

|                           |                                                               |
| ------------------------- | ------------------------------------------------------------- |
| 빈칸 더블클릭             | 그래프 프로퍼티                                               |
| 스페이스 / 탭             | 노드 검색 및 추가 가능                                        |
| 스페이스                  | 2D View에서 타일링모드 온오프                                 |
| R/G/B/A/C                 | 2D View - Red/Green/Blue/Alpha/Color                          |
| Cmd + Shift + 우클릭 이동 | 3D View에서 배경 이동                                         |
| 1                         | Standard 단일 노드라인                                        |
| 2                         | Material 그룹 노드라인                                        |
| 3                         | Compat Material 그룹 노드라인                                 |
| D                         | 노드 축소                                                     |
| X                         | 노드 라인 크로스                                              |
| Shift + X                 | Bitmap 노드에서 색상 크로스                                   |
| Cmd + E                   | 노드 Edit                                                     |
| Ctrl                      | 누른 상태에서 노드 라인을 드래그하면 노드 라인 복사           |
| Shift                     | 누른 상태에서 노드 라인 드래그하면 노드라인이 그룹지어서 이동 |
| Alt                       | 노드 라인 클릭시 Dot 추가.                                    |
| Alt                       | Dot노드 드래그시 걸쳐있는 노드 라인 합치기                    |
| Alt                       | 노드 라인 접합부 클릭시 연결 해제                             |
| Delete                    | 노드 삭제(연결 라인은 보존)                                   |
| Backspace                 | 노드 삭제(연결 라인도 삭제)                                   |

Node information > Display timings
https://helpx.adobe.com/substance-3d-designer/interface/the-graph-view.html




## 노드

|         |                                |
| ------- | ------------------------------ |
| Frame   | 그룹핑 및 주석                 |
| Pin     | F2로 바로 갈 수 있음           |
| Dot     | 연결점 / **포탈로도 사용가능** |
| Comment | 주석                           |

Output
  export시 그룹핑 가능
Safe Transform
  타일링 유지 Transform
Shape Extrude
  Shape를 확장
Multi Dir. Warp
  여러 방향으로 블랜드
Vector Morp
Vector Warp
Blur보다는 Blur HQ
Slope Blur GrayScale
  블러와 블랜드를 동시
Tile Generator
Tile Sampler
  가로/세로 랜덤하게 석을때 사용


Highpass GrayScale
  대비감을 줄이고 경계를 강조 - Levels랑 같이 써서 경계추출 => Edge Detect

Histogram Range
Histogram Shift
Histogram Scan
  Levels보다 단순하지만 직관적
Histogram Select
  마스크에서 일부 영역이 필요시

Levels
  입력 이미지의 특정 범위 내에서 픽셀 값을 조정하여 이미지의 전반적인 톤을 변경
Curve
  곡선을 조절하여 이미지를 수정

Curvature
Curvature Sobel 엣지
Curvature Smooth 부드러운


/Applications/Adobe\ Substance\ 3D\ Designer/Adobe\ Substance\ 3D\ Designer.app/Contents/Resources/templates

## art

- https://realtimevfx.com/t/rain-drop-effect-in-unity/5307

## 텍스쳐 분석

HBAO Horizon-Based Ambient Occlusion
RTAO Ray Traced Ambient Occlusion

## 2D Fire Projectile Shader Graph

심리스텍스쳐제작(포토샵) 베이스텍스쳐에 사각형으로 심리스 베이스를 잡음

불꽃 진행방향이 좀 특이했음

진행방향 왼쪽
불꽃방향 왼쪽
디솔브방향 오른쪽

3겹으로 쌓아올리니 그럴싸함(코어/주변/연기)



## 2D Wind Vegetation Shader Graph (Vertex Movement Tutorial)
전체이미지를 움직이는게 아닌 uv를의 v를 상단 부분의 마스크로 이용

## 2D Dissolve Shader Graph
A : 노이즈에 스탭을 줘서 알파값으로 디솔브
B : 노이즈 스탭값을 추가한것
C : 아웃라인시킨것(B - A)
[ColorUsage(true, true)] 어트리뷰트로 intensity 적용가능한 색상편집다이얼로그

## 2D Pixel Art Shader Graphs
픽셀라이즈된 이미지를 시간에 따른 노이즈로 흩뜨린것으로 나뭇가지 바람에 날리는 효과(2D)

## 3D Magical Portal
float2 Center      = 0.5;
float  RadialScale = 1;
float  LengthScale = 1;
float2 delta = UV - Center;
float radius = length(delta) * 2 * RadialScale;
float angle = atan2(delta.x, delta.y) * 1.0/6.28 * LengthScale;
float2 polarCoord = float2(radius, angle);

polarCoord.x : 원
polarCoord.y : 우측

outerCircle = smoothstep(_CircleClip , _CircleClip  + _Feather, polarCoord.x);
edge1 = _CircleClip - _RingWidth;
edge2 = edge1 + _Feather;
innerCircle = smoothstep(edge1, edge2, polarCoord.x);
ring = innerCircle - outerCircle

- polarCoord를 적용하기 위해 포토샵으로 텍스쳐 제작
  - 일반 노이즈에 polarCoord를 적용하면 씸리스가 안됨.

포토샵
Filter> Render> Clouds
Filter> Blur> Motion Blur(angle:45, distance:100)
Filter> Other> Offset을 조정하면서 접합부가 보이면 뭉대겨서 접합부를 안보이게 만들어 줘야함.


## 3D Stylized Water Shader - 중요

depthFade = saturate((SceneDepth(Eye) - ScreenPosition(Raw).a) / _Distance);
waterGradientColor = lerp(_SurfaceColor, _DeepColor, depthFade);

noiseNormal = GradientNoise를 반대방향으로 2개를 만들고,  NormalFromHeight로 노말을 구해 노말을 블렌드한다
waterNormalStrength = lerp(0, _WaterNormalStrength, depthFade);
waterNormal = saturate(NormalStrength(noiseNormal, waterNormalStrength));
waterSceneColor = SceneColor((noiseNormal  * 0.1 * _RefractionStrength) + ScreenPosition(Default))
waterColor = lerp(waterSceneColor, waterGradientColor, waterGradientColor.a); 

폼은
waterFormNoise = GradientNoise를 움직이고
waterFormNoiseStep = step(waterFormNoise, depthFade * 2)
waterFormColor = lerp(waterGradientColor, _FormColor, waterFormNoiseStep);
finalWaterColor = lerp(waterColor, waterFormColor, waterFormColor.a);

## Sub-Surface Scattering (SSS) Shader Graph
NdotV 로 림을 만들고 LightIntensity를 곱해 SSS를 만들고
(1 - HeightMap)과 곱해 메인칼라에 더해준다

blender를 이용 Thinknessmap
- UV Editing Tab
  Image> New> Thickness로 이름
- shading tab
노드들 지우고
AmbientOcclusion(Inside 체크 및 Distance 조정)
ImageTexture 노드에 앞서만든 Thickness 선택

- Render Tab
Bake Type> Emit
Max Ray Distance> 0.2
Bake버튼
- UV Editing Tab
  Image> Save As> Thickness.png

## Triplanar Shader Graph

텍스쳐를 입히는것이 오브젝트공간이 아닌 월드공간으로 지형에 어울리는것을 배치할때 자연스럽게

[assetstore:Valley Gray Cliff(무료)](https://assetstore.unity.com/packages/3d/props/exterior/valley-gray-cliff-203730)

height = PositionWS.y
heightSmooth = smoothstep(_2ndTextureHeightBlend - 1, _2ndTextureHeightBlend + 1, height)
heightBlendVal = smoothstep(0, 1 - _2ndTextureThreshold, heightSmooth * normalWS.y)
color = lerp(_MainTex, _2ndTex, heightBlendVal)


Extra content
void Unity_RadialShear_float(float2 UV, float2 Center, float Strength, float2 Offset, out float2 Out)
{
    float2 delta = UV - Center;
    float delta2 = dot(delta.xy, delta.xy);
    float2 delta_offset = delta2 * Strength;
    Out = UV + float2(delta.y, -delta.x) * delta_offset + Offset;
}

51. Colors Theory (Choose the most pleasing color combinations of color) 중요
Shade : add dark
Tint : add White
Tone : add Gray

MonoChromatic 하나
Complementary 하나 그리고 반대
splitcomplementary 하나 그리고 반대편 양쪽 2개
Triadic             3등분
Analogous 주변색
TetradicColors 양쪽2개 반대편 양쪽 2개


== 
- 하나의 Dominant(지배적인) 색 선택
- 되도록 적은 색 선택
https://color.adobe.com/



https://www.slideshare.net/LeeJungpyo/kgc2014-jplee-allegorithmic


## 머티리얼

https://www.artstation.com/learning/courses/xQY/why-you-are-struggling-to-learn-substance-designer/chapters/P5pA/breaking-an-idea-down

머티리얼 분석시
낮은 높이에서 높은 높이 순으로 질감 분류



## UI Making

- [Card Game ART | Frame Design (Substance Designer) Procedural GUI Elements - Fantasy Game](https://youtu.be/9DPftVVz2_I?si=vR_gYbNvknWIuUvd)

회전과 같은 3D UI 만들때 Substance Designer를 이용할 수 도 있겠다.


## ---------


/Applications/Adobe Substance 3D Designer/Adobe Substance 3D Designer.app/Contents/MacOS/
sbsbaker
sbscooker
sbsrender
sbsupdater


SAT(Adobe 3D Substance Automation Tool Kit)
https://adminconsole.adobe.com/ 엔터프라이즈 버전에서 사용가능

https://helpx.adobe.com/substance-3d-sat/setup-and-getting-started.html


---

## [20 Tips I Wish I Knew When I Started Substance Designer](https://www.youtube.com/watch?v=Np95Efw57uQ)


0:00:08 - 1 - YUp Mask
(1 - NormapMap.g) 과 블랜드하여 색상을 입히면 표면 상단에 뭔가 낀(이끼) 효과를 낼 수 있다.

0:03:02 - 2 - Blend Crop
마스크맵을 Blend를 활용해서 만들 수 있다.
Ramp / Histogram

0:04:27 - 3 - Sample Image Inputs
Gradient Map에서 Pick Gradient하는 대신
텍스쳐랑 Gradient Linear와 를 Gradient(dynamic) 하면 좀 더 깔끔한 색을 얻을 수 있다.

0:08:01 - 4 - Water Damage Mask
Cloud노이즈를 조정해서 Roughness에 적용하면 물 효과를 얻을 수 있다.

0:10:18 - 5 - Native Invert/Auto Level
Level역시 Invert와 같이 활용가능. (버튼 있음)

0:11:19 - 6 - Custom Voronoi
일반적인 Cell로는 뭔가 거리가 비슷비슷해보임

Cloud를 Tile Sampler로 패턴으로 넘김
Tile Sampler를 인풋2로
Threshold를 거친것을 인풋 1로
 Distance로 넘겨서 Maximum Distance을 256으로

0:14:58 - 7 - Auto Bevel
Tile Sampler에서 Bevel을 사용할때 Distance를 최대치로 함
Tile Sampler의 X/Y수치를 조절하면 Bevel에서 Distance가 최대치가 아닐때 타일사이 거리가 벌어짐.
단, Bevel에서 Distance가 최대치면 너무 밝아지는데 Auto Levels를 사용하면 됨.


0:16:38 - 8 - RRGRandom Masks
GrayScale이냐 RGBA냐 - ex) Flood Fill to Random Color 후 Distance 다음 RGBA Split하면 마스크를 4개 얻을 수 있음. 노드 사용이 줄어들음.

0:18:10 - 9 - High Freq. Normal Preview
GrayScale에서 차이점을 찾기 힘들어서 시각적 확인용으로 Normal을 사용.

0:19:51 - 10 - SubGraphs
pass

0:24:04 - 11 - MakeItTile Precision
Cloud를 Transform으로 확대하면 타일링이 깨지는데 이때 Make Tile Photo Gray를 쓰면 보간해줌

0:26:27 - 12 - Keep Ratio
Tile Generator에서 Size Mode에 Keep Ratio모드가 있다.

0:28:09 - 13 - FloodFill Distances
작은 균열에는 Flood Fill을 쓰는 게 좋다. 하지만 그냥 쓰게 되면 검은 연결자국이 남는다
Flood Fill to Random GrayScale를 소스 입력으로 Distance를 사용해주자. 마스크는 원래 자국으로. 그러면 연결자국이 없어진다.

0:30:40 - 14 - Mirrored Parameters
Tilemap Sampler 가 2개일때 한쪽의 X/Y수치를 바꾸면 다른 한쪽도 변경하는게 불편하다.
Expose Parameter로 매개변수를 추출하고 Use existing graph input을 사용하면 된다.

0:33:03 - 15 - RGBA 2d Preview
pass

0:33:59 - 16 - Slope Blur Inflate
원본과 Blur HQ GrayScale된걸 Slope Blur에 넣어 모양을 부풀릴 수 있다.

0:35:15 - 17 - Pre-Rotations
풀 같이 회전하는 것들은 회전 원점을 생각해서 정중앙이 아닌 미리 위치를 조금 올려놓자

0:38:04 - 18 - FloodFill Curvature Mask

Cell을 가지고 돌맹이를 만들다 보면 중앙 마스크를 얻기 힘듬
단순 Cell을 Edge Detect한걸 가지고 하는게 아니라
Normal이랑 Culvature Sobel 해주고 Histogram Scan으로 엣지를 얻은걸 A
A에다가 Flood Fill 다음 Flood Fill to Random GrayScale한것을 B
A랑 B를 Distance에 입력

마스크를 얻을 것이랑 Blend(Multiply)를 함

0:41:00 - 19 - Portal Node
pass

0:43:53 - 20 - Custom Nodes

Tile Sampler를 예로들어 패턴 입력이 6개가 최대인데 노드를 수정해서 입력을 추가할 수 있다.