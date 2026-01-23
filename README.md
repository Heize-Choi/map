a23map.html - 가장 최신 버전 맵 (모선 정보 업데이트)
png - 아이콘 이미지
(hospitals, military_categorized).geojson : 기관 정보
(hospital)_links.geojson, (military)_links_categorized.geojson : 어떻게 연결되었는지에 대한 정보
substation2.geojson : 모선 정보

py파일
hospital.py :OSM에서 병원 정보 받아와서 csv파일로 저장 -> 이후 상급종합병원은 수작업으로 전처리
military.py : OSM에서 군사시설 정보 받아와서 csv파일로 저장
military_preparing.py : 군사시설 csv파일을 카테고리로 분류 + 전처리 -> 이후 duplicate 등은 수작업 필요..
preparing_data.py: csv파일을 geojson파일로 변환하여 html로 들어가기 쉽도록 변경 및 거리 계산 후 파일저장

main.py : 변전소 업데이트 코드(현재 사용 x)
json to csv : military json 파일을 csv  파일로 변환하기 위함
