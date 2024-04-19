![gmm_cosine_top10](https://github.com/YOOHYUNJUNE/music_rec_GMM/blob/master/output.png)

GMM(gaussian mixture model)군집화(clustering)를 이용한 유사 음원 추천

한계
- 군집화에 필요한 특정 컬럼을 5개로 정했으나, 정확한 컬럼 선정의 근거 빈약(단순히 시각화가 잘 되어서)
- 음악적 특성이 곡마다 너무 다양해서, 같은 군집끼리 명확한 장르가 나누어지지 않음


순서
- 스포티파이 API를 통해 음원 특성 추출
- 음원 데이터 GMM으로 6개 군집화(Kmeans는 군집간 침범이 심하고 제대로 군집화 되지 않았음)
- 예시 음원과 같은 군집내 코사인 유사도가 높은 곡들 추출(반드시 군집을 동일하게 할 필요는 없음)
