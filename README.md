# 샌프란시스코 도시 범죄율을 낮추기 위한 방안 마련 프로젝트

이 프로젝트는 샌프란시스코 범죄 데이터를 분석하고 범죄 예방 및 대응 전략을 개발하는 데 관한 내용을 다룹니다.

- 데이터 출처 : [Kaggle 링크](https://www.kaggle.com/competitions/sf-crime/data)
- 노션 페이지 : [Notion 링크](https://www.notion.so/gowiththeflaw/TEAM-997b9a91dbc2443fb8240ab5dc33083b?pvs=4)

## 팀 소개

- 팀 이름 : 라마단
- 팀장 : [채화정](https://github.com/HwajeongChae)
- 팀원 : 
    - [이수](https://github.com/prunusblssm)
    - [정영진](https://github.com/jyj1206)
    - [정용은](https://github.com/JeongYongEun)


## 시작하기

아래의 지침을 참고하여 프로젝트를 실행할 수 있습니다.


### 참고
메인 프로젝트 파일인 `TEAM_LamaDan_FullCode.ipynb`의 경우 용량 초과로 lfs를 사용했습니다.

[lfs 참고 링크](https://docs.github.com/ko/repositories/working-with-files/managing-large-files/installing-git-large-file-storage)를 활용하여 lfs 관련 필요 파일을 설치하고
```
git lfs pull
```
위의 코드를 이용하여 사용바랍니다.


### 데이터 경로 설정

주 데이터는 Kaggle에서 제공하는 `San Francisco Crime Classification` 문제의 `train.csv`만을 다루고 있습니다.

1. 데이터를 다운로드하고 저장할 디렉토리를 만듭니다.

2. 아래 링크에서 샌프란시스코 범죄 데이터를 다운로드합니다.
   [데이터 다운로드 링크](https://www.kaggle.com/competitions/sf-crime/data?select=train.csv.zip)

3. 다운로드한 데이터를 프로젝트의 해당 디렉토리에 저장합니다.

4. 메인 코드인 `TEAM_LamaDan_FullCode.ipynb`의 path 부분을 수정합니다.


### 외부 데이터 불러오기

이 프로젝트에서는 지도 데이터 시각화를 위한 외부 데이터를 사용합니다. 외부 데이터를 불러오는 방법은 다음과 같습니다.

1. 외부 데이터를 다운로드하고 저장할 디렉토리를 만듭니다.(외부 데이터의 경우 data 폴더 하위에 존재)

2. 다운로드한 외부 데이터를 프로젝트에 불러옵니다.


### 프로젝트 실행 과정 요약

1. Jupyter Notebook 또는 주피터 랩을 사용하여 `TEAM_LamaDan_FullCode.ipynb` 파일을 실행합니다.

2. 데이터 경로를 설정하고 필요한 외부 데이터를 불러옵니다.

3. EDA, 지도 데이터 시각화, 분류 모델링 등의 작업을 진행합니다.

4. 결과 및 결론을 도출합니다.


## 시스템 요구 사항

이 프로젝트를 실행하기 위해서는 다음 요구 사항이 필요합니다:

- Python 3.9
- 필요한 Python 패키지 및 버전
```
    Matplotlib 버전: 3.4.3
    Seaborn 버전: 0.11.2
    Scikit-learn 버전: 1.0
    Imbalanced-learn 버전: 0.8.1
    LightGBM 버전: 3.3.0
    XGBoost 버전: 1.4.2
    TensorFlow 버전: 2.6.0
    Geopandas 버전: 0.10.1
    Folium 버전: 0.12.1
```
- Jupyter Notebook 또는 주피터 랩


## 참고 자료 및 외부 데이터 출처

- GIS 외부 데이터 (Data SF - https://data.sfgov.org/)
* 샌프란시스코 경찰서 위치
> 출처: https://data.sfgov.org/Public-Safety/Police-Stations-2011-/rwdu-9wb2  
> 파일명 : sf_Police_Stations.csv
* 샌프란시스코 경찰서별 담당구역
> 출처: https://data.sfgov.org/Public-Safety/Current-Police-Districts/wkhw-cjsf  
> 파일명 : sf_Police_Districts.geojson
* 샌프란시스코 랜드마크
> 출처: https://data.sfgov.org/Geographic-Locations-and-Boundaries/Landmarks/rzic-39gi  
> 파일명 : sf_Landmarks.geojson



## 기여 및 문의 사항

이 프로젝트에 기여하거나 문의 사항이 있으면 [GitHub 이슈](https://github.com/AiffelTeamLamaDan/SanFran_Crime_Decline/issues)를 통해 문의하세요.
