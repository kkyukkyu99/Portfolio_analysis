# Portfolio
Portfolio_analysis

***
<h2>#1. Project - 우리나라 인구 소멸위기 지역 분석</h2> 

- 배경
<p>대한민국은 지역별 인구 불균형과 인구 소멸 위기에 있는 나라입니다.<br/>
  따라서, 소멸 위기 지역 분류와 소멸 위기 비율을 분석하고 시각화함으로써 지역 불균형과 인구 소멸 위기의 심각성을 강조하고 싶습니다.</p>
<p>소멸 위기 지역의 정의: 20~39세 여성 인구가 65세 이상 노인인구 절반에 미달인 지역<br/>
출처: 한국 고용정보원  한국의 지방 소멸에 관한 7가지 분석
</p>

- Summary
	
	1. Data Source
		- https://kosis.kr/statisticsList/statisticsListIndex.do?vwcd=MT_ZTITLE&menuId=M_01_01#content-group
	
	2. Data Preprocessing
		- 다중컬럼으로 인해 생성 된 인덱스 결측치 변환
		- 90세 이상 데이터의 X 결측치 0으로 대체
		- 컬럼명 변경
			
	3. Feature Engineering & EDA
	  	- 20~39세의 인구와 65세 이상의 인구로 연련대 통합 및 파생변수 추가
		- 연령별 인구 수로 지역별 소멸비율 파생변수 추가
	
	4. Visualization
		- 시각화를 위한 전처리 
			- 다중 컬럼은 하나의 컬럼으로 합치기
    		- 다중 인덱스는 컬럼으로 조정
			- 지역별 고유 ID 생성 및 지도 분할 json파일과 연동<br/>
		![소멸 지역 시각화]()
		![소멸 비율 시각화](https://github.com/kkyukkyu99/Portfolio_analysis/blob/main/%EC%86%8C%EB%A9%B8%EB%B9%84%EC%9C%A8%20%EC%8B%9C%EA%B0%81%ED%99%94.PNG)	
	
	5. Report
		- 광역시 보다 지방 지역에 소멸 위기가 더 심각하다는 것을 알 수 있습니다.
