(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> pwd

Path
----
C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project...


(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> ls


    디렉터리: C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigd
    ata-project-a-20242884


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-03-20  오후 12:33                2_week
d-----      2026-03-20  오후 12:27                3_week
d-----      2026-03-20  오후 12:58                als
d-----      2026-03-20  오전 10:03                venv
-a----      2026-03-20  오후 12:24             72 .env
-a----      2026-03-20  오전 10:42            162 .gitignore     
-a----      2024-05-14   오후 2:56        2103037 Air_Quality.cs 
                                                  v
-a----      2026-03-13  오후 12:53           1035 app.py
-a----      2026-03-13  오전 10:33           1854 requirements.t 
                                                  xt


(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> cd 2_week   
(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884\2_week> cd ..    
(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> mkdir als


    디렉터리: C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigd 
    ata-project-a-20242884


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-03-20  오후 12:59                als


(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> cat app.py
import streamlit as st
import pandas as pd
# ?섏씠吏 ?ㅼ젙
st.set_page_config(page_title="鍮낅뜲?댄꽣 遺꾩꽍 ?꾨줈?앺듃", page_icon="?뱤")
# ?쒕ぉ
st.title("鍮낅뜲?댄꽣 遺꾩꽍 ?꾨줈?앺듃")
st.write("泥?踰덉㎏ Streamlit ?깆엯?덈떎!")
# 援щ텇??
st.divider()
# 媛꾨떒???곗씠?고봽?덉엫 ?쒖떆
st.subheader("?섑뵆 ?곗씠??)
data = {
 "?대쫫": ["源泥좎닔", "?댁쁺??, "諛뺣???, "?뺤닔吏?, "理쒖???], 
 "?숇뀈": [3, 3, 3, 3, 3],
 "?꾧났": ["AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??, "AI?뚰봽?몄썾??],
 "Python?먯닔": [85, 92, 78, 95, 88]
}
df = pd.DataFrame(data)
st.dataframe(df, use_container_width=True)
# 媛꾨떒??李⑦듃
st.subheader("Python ?먯닔 李⑦듃")
st.bar_chart(df.set_index("?대쫫")["Python?먯닔"])
# ?ъ씠?쒕컮
st.sidebar.header("?ㅼ젙")
st.sidebar.write("???곸뿭? ?ъ씠?쒕컮?낅땲??")
name = st.sidebar.text_input("?대쫫???낅젰?섏꽭??)
if name:
 st.sidebar.write(f"?덈뀞?섏꽭?? {name}??")
(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> cp 2_week\source\aaa.md
(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> mv 2_week\source\aaa.mv
mv : 'C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-proj
ect-a-20242884\2_week\source\aaa.mv' 경로는 존재하지 않으므로 찾 
을 수 없습니다.
위치 줄:1 문자:1
+ mv 2_week\source\aaa.mv
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (C:\Users\6-112\.  
   ..k\source\aaa.mv:String) [Move-Item], ItemNotFoundExceptio   
  n
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell  
   .Commands.MoveItemCommand

(venv) PS C:\Users\6-112\Desktop\빅데이터분석프로그래밍\bigdata-project-a-20242884> rm als