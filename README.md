### 본 내용은 R의 학습 방향을 정리하고자 작성한 노트입니다. (2018.06.13.)
### 작성자: 홍승재
 

#### 개요는 아래와 같습니다. &#128526;

1. R과 R Studio에 대한 필수 개념 및 기본 함수 정리
    + R/R-studio 설치 (~~해당 내용은 아주 많은 블로그에서 찾을 수 있으므로 작성하지 않을 계획~~)
    + 기본 내장 함수를 바탕으로 한 내용 ([R을 이용한 데이터 처리 실무, 서민구][1]에서 많은 내용을 참조하였습니다.) 
        + Data Type
        + 제어문, 연산, 함수
        + 벡터 연산
        + 데이터 조작
        + 기본 데이터
        + 시스템 세팅 관련
            + options, Sys.setlocale 등


2. 핵심 패키지 정리 (패키지와 관련한 내용은 사용했던 패키지 위주로 차츰 업데이트를 할 예정입니다) 
    + [(R 패키지 리스트 CRAN)](https://cran.r-project.org/web/packages/available_packages_by_name.html) 
    + [(R cheatsheet provided by R-studio)](https://www.rstudio.com/resources/cheatsheets/) 
        + 사실 이 cheat sheet만 봐도 어느정도 감만 있으면 다 할 수 있습니다 - 주요 패키지와 관련한 cheat sheets이 요약되어 있으니 참고 하면 됩니다
    + [수학 연산](https://cran.r-project.org/web/views/NumericalMathematics.html) - R은 기본적으로 통계 분석을 위한 프로그램이기 때문에 Python의 NumPy, SciPy와 같은 별도의 특화된 라이브러리가 있기 보다는 그 자체가 수학적 연산에 강한 측면을 갖고 있는 것 같습니다. 
    + 이러한 측면 때문에 R와 Python은 데이터 처리 과정에서도 서로 각기 다른 모습을 보이기도 한다. 
        + [matrix](https://cran.r-project.org/web/packages/Matrix/)

    + 데이터 처리
        + [doBy](https://cran.r-project.org/package=doBy)
        + [plyr](https://cran.r-project.org/web/packages/plyr/)
        + [stringr](https://cran.r-project.org/web/packages/stringr/)
        + [doParallel](https://cran.r-project.org/package=doParallel)
        + [foreach](https://www.rdocumentation.org/packages/foreach/versions/1.4.4)
        
    + 시각화
        + [ggplot2](https://cran.r-project.org/web/packages/ggplot2/ggplot2.pdf)
        + [knitr](https://cran.r-project.org/web/packages/knitr/)
        + [scatterplot3d](https://cran.r-project.org/web/packages/scatterplot3d/)
    + 분석
        + 통계 & 시뮬레이션
            + [forecast](https://cran.r-project.org/web/packages/forecast/)
            + [survival](http://cran.r-project.org/web/packages/survival/survival.pdf)
        + 사회 연결망 분석
            + [igraph](https://cran.r-project.org/web/packages/igraph/)
            + [sna](https://cran.r-project.org/web/packages/sna/sna.pdf)
            + [statnet](http://www.statnet.org/)
            + [Network Visualization과 관련한 전반적인 설명이 담긴 블로그](http://kateto.net/network-visualization)
        + 머신러닝 & 딥러닝
            + [kernlab](https://cran.r-project.org/web/packages/kernlab/)
            + [tree](https://cran.r-project.org/web/packages/tree/)
        + 텍스트 마이닝 & 분석
            + [tm](https://cran.r-project.org/web/packages/tm/tm.pdf)
            + [KoNLP](https://cran.r-project.org/web/packages/KoNLP/vignettes/KoNLP-API.html)
    + 크롤링
        + [RCurl](https://cran.r-project.org/web/packages/RCurl/)
        + [XML](https://cran.r-project.org/web/packages/XML/XML.pdf)
        + [rvest](https://cran.r-project.org/web/packages/rvest/rvest.pdf)
    + 데이터베이스
        + [RSQLite](https://cran.r-project.org/web/packages/RSQLite/)
    + 기타
        + [foreign](https://cran.r-project.org/web/packages/foreign/)
        + [devtools](https://cran.r-project.org/web/packages/devtools/)
        
---        
#### Reference List 

1. [데이터 사이언스 스쿨 - R 버젼](https://datascienceschool.net/view-notebook/10287029287b41b4a382f1029e6e4972/)

2. [useful packages](https://support.rstudio.com/hc/en-us/articles/201057987-Quick-list-of-useful-R-packages)

3. [Top 100 packages in 2013](https://www.r-statistics.com/2013/06/top-100-r-packages-for-2013-jan-may/)

4. [R에 대한 소개 (한국어 번역)](https://r-forge.r-project.org/scm/viewvc.php/*checkout*/www/manual/R-intro-ko.html?revision=1220&root=ihelp&pathrev=1271)

#### 기타 참고 도서
1. Teetor, Paul. (2011). *R Cookbook*. O'Reilly

2. Cotton, Richard. (2013). *Learning R*. O'Reilly

3. Schutt, Rachel & O'Neil, Cathy. (2014). *Doing Data Science*. O'Reilly

4. James, Gareth., Witten, Daniela., Hastie, Trevor., & Tibshirani, Robert. (2013). *An Introduction to Statistical Learning with Applications in R*. Springer

5. Gardener, Mark. (2015). *The Essential R Reference*. Wiley

6. Kolaczyk, E. D. & Csardi, G. (2009) *Use R!: Statistical Analysis of Network Data in R*. Springer

7. Falissard, Bruno. (2012). *Analysis of Questionnaire Data with R*. CRC Press

8. Kleiber, Christian & Zeileis, Achim. (2008) *Use R!: Applied Econometrics with R*. Springer

9. Luke, Douglas A. (2016). *Use R!: A User's Guide to Network Analysis in R* Springer



[1]: http://r4pda.co.kr/pdf/r4pda_2014_03_02.pdf
