# Statistical Analysis on Covid-19 Microarray Dataset with R
## Buğra 17.01.2021 ( ENGLISH - TÜRKÇE )
## English
In this R project I applied some statistical methods to analize covid-19 microarray dataset. 
I explained all the steps and code lines in .Rmd file. I made it markdown file , so you can see the each processes.
##

### Boxplot Visualization Before Normalization
![beforenormalize](https://user-images.githubusercontent.com/49213911/105470905-30092200-5cab-11eb-8d6f-621b01f89618.png)

### Boxplot Visualization After Normalization
![afternormalize](https://user-images.githubusercontent.com/49213911/105470924-38615d00-5cab-11eb-9b8b-ba1c84d03844.png)

### Heatmap Visualization
In each heatmap, the columns represent gene expression profile for the patients while the rows represent the expression profiles for each gene across all patients.

![heatmap](https://user-images.githubusercontent.com/49213911/105470980-4b742d00-5cab-11eb-9cf5-9672d9f75626.png)

### Cluster Dendrogram Visualization
![clustering](https://user-images.githubusercontent.com/49213911/105471044-60e95700-5cab-11eb-8494-2cb7dc32f2cf.png)

## Required R packages: 
### [limma](https://bioconductor.org/packages/release/bioc/html/limma.html)
### [dplyr](https://www.rdocumentation.org/packages/dplyr/versions/0.7.8)
### [ggplot2](https://cran.r-project.org/web/packages/ggplot2/index.html)
### [RColorBrewer](https://cran.r-project.org/web/packages/RColorBrewer/index.html)
##
## General Information on the Subject 
### What is Microarray?
Microarray is a high-tech technique used for the detection of inclusions and additions that are too small to be observed with a microscope.
### Why do we use Microarray?
Microrarray studies yield a genomic profile based on thousands of gene expressions for each patient.
![whdoweuse](https://user-images.githubusercontent.com/49213911/105472702-5039e080-5cad-11eb-956d-ef96ff954e32.png)
### What is gene expression profile?
In the field of molecular biology, gene expression profile is the measurement of the activity of thousands of genes at once to create a global picture of cellular function. These profiles can, for example, distinguish between actively dividing cells or show how the cells respond to a particular treatment.

![geneexpression](https://user-images.githubusercontent.com/49213911/105472800-66e03780-5cad-11eb-918e-2afa14a5d610.jpg)

### Why do we use gene expression profile?
A gene expression profile may be used to find and diagnose a disease or condition or to see how well the body responds to treatment.

### What is the aim of doing statistical analysis on Microarray Datasets?
1- Identify the changes in gene sequences that are most often associated with particular diseases

2- Determine how often individuals with a particular mutation actually develop breast cancer.

3- Microarrays can also be used to study the extent to which certain genes are turned on or off in cells and tissues.

### We want to extract what?

Microarray statistical analysis wants to identify genes with significantly changed gene expression.
##
### 9 Statistical Analysis Approaches to Microarray Dataset
![approaches](https://user-images.githubusercontent.com/49213911/105473209-e1a95280-5cad-11eb-8e49-bf77c0cebcf7.png)
##
### T-test

The t test is a simple, statistically based method for detecting differentially expressed genes . In replicated experiments, the error variance  can be estimated for each gene from the log ratios, and a standard t test can be conducted for each gene; the resulting t statistic can be used to determine which genes are significantly differentially expressed.

### BoxPlot

Box plots allow you to assess if the scale and distribution of the data on different arrays is comparable. Differences in shape or center of the boxes indicate that normalization of the data is required.

### Normalization

Normalization is the process of removing some sources of variation which affect the measured gene expression levels. Normalization plays an important role in the earlier stage of microarray data analysis. The subsequent analysis results are highly dependent on normalization.

The purpose of normalization is to make the intensities for features that are not differentially expressed similar across the arrays.
Systematic differences between the samples that are due to noise rather than true biological variability should be removed in order to make biologically meaningfull conclusions about the data.

![beforeafterbox](https://user-images.githubusercontent.com/49213911/105473321-0c93a680-5cae-11eb-9739-bb62a5eb031b.png)

### ANOVA

Usually the experimenter wants to know which genes  are actively regulated during treatment in two cell lines, or  wants some criterion for selecting those that are differentially  regulated among groups. These questions belong in the  tradition of analysis of variance (ANOVA).

In health research, effect size can be used in statistical techniques such as regression models, multi-directional analysis of variance (ANOVA) or multivariate analysis of variance (MANOVA).

### Volcano Plot

The ‘volcano plot’ arranges genes along dimensions of biological and statistical significance. The researcher can then make judgements about the most promising candidates for follow-up studies, by trading off both these criteria by eye.

![volcanoplot](https://user-images.githubusercontent.com/49213911/105473441-2df49280-5cae-11eb-8009-e8878409092b.png)

### P-Value

The P-value can serve as a probability measure to select differentially expressed genes from a pre-specified significance level (cutoff threshold). 
So whether there is a difference between genes, we can turn it into a probability measure.

### Permutation Testing

Permutation testing is an approach that is widely applicable  and copes with distributions that are far from Normal.
This  approach is particularly useful for microarray studies because  it can be easily adapted to estimate significance levels for many  genes in parallel.

A permutation-based p-value tells how rare that test statistic  is, among all the random partitions of the actual samples into  pseudo-treatment and pseudo-control groups.

### Empirical Bayes Methods

Empirical Bayes methods are procedures for statistical inference in which the prior distribution is estimated from the data. This approach stands in contrast to standard Bayesian methods, for which the prior distribution is fixed before any data are observed.
Bayesian approaches make assumptions about the parameters  to be estimated (such as the differences between gene levels in  treatment and control groups).

### MMM(Mixture Model Method)

An important and common task in analyzing microarray data is to identify genes with altered expression under two experimental conditions. We propose a nonparametric statistical approach, called the mixture model method (MMM), to handle the problem when there are a small number of replicates under each experimental condition. Specifically, we propose estimating the distributions of a t -type test statistic and its null statistic using finite normal mixture models. 

### How can we apply stastical analysis to microarray data?

1-Reading raw data

2-Quality Check

3-Normalization 

4-Filtering 

5-Selection of differentially expressed genes

6-Comparison of selected lists

7-Analysis of Biological Significance.

##

## Türkçe
Bu R projesinde covid-19 mikroarray veri setini analiz etmek için bazı istatistiksel yöntemler uyguladım.
.Rmd dosyasındaki tüm adımları ve kod satırlarını anlattım. Markdown dosyası yaptım, böylece her işlemi görebilirsin.
##

### Normalleştirmeden Önce Kutu Grafiği Görselleştirme
![beforenormalize](https://user-images.githubusercontent.com/49213911/105470905-30092200-5cab-11eb-8d6f-621b01f89618.png)

### Normalleştirme Sonrası Kutu Grafiği Görselleştirme
![afternormalize](https://user-images.githubusercontent.com/49213911/105470924-38615d00-5cab-11eb-9b8b-ba1c84d03844.png)

### Isı Haritası Görselleştirme
Her ısı haritasında, sütunlar hastalar için gen ekspresyon profilini temsil ederken, satırlar tüm hastalarda her gen için ekspresyon profillerini temsil eder.

![heatmap](https://user-images.githubusercontent.com/49213911/105470980-4b742d00-5cab-11eb-9cf5-9672d9f75626.png)

### Küme Dendrogram Görselleştirme
![clustering](https://user-images.githubusercontent.com/49213911/105471044-60e95700-5cab-11eb-8494-2cb7dc32f2cf.png)

## Gerekli R paketleri: 
### [limma](https://bioconductor.org/packages/release/bioc/html/limma.html)
### [dplyr](https://www.rdocumentation.org/packages/dplyr/versions/0.7.8)
### [ggplot2](https://cran.r-project.org/web/packages/ggplot2/index.html)
### [RColorBrewer](https://cran.r-project.org/web/packages/RColorBrewer/index.html)
##
## Konuyla İlgili Genel Bilgiler
### Microarray nedir?
Mikroarray, mikroskopla gözlemlenemeyecek kadar küçük inklüzyonların ve eklemelerin saptanması için kullanılan yüksek teknoloji bir tekniktir.
### Neden Microarray kullanıyoruz?
Mikrorarray çalışmaları, her hasta için binlerce gen ifadesine dayalı bir genomik profil verir.
![whdoweuse](https://user-images.githubusercontent.com/49213911/105472702-5039e080-5cad-11eb-956d-ef96ff954e32.png)
### Gen ifade profili nedir?
Moleküler biyoloji alanında, gen ekspresyon profili, hücresel işlevin küresel bir resmini oluşturmak için aynı anda binlerce genin aktivitesinin ölçülmesidir. Bu profiller, örneğin aktif olarak bölünen hücreleri ayırt edebilir veya hücrelerin belirli bir tedaviye nasıl tepki verdiğini gösterebilir.

![geneexpression](https://user-images.githubusercontent.com/49213911/105472800-66e03780-5cad-11eb-918e-2afa14a5d610.jpg)

### Neden gen ekspresyon profilini kullanıyoruz?
Bir hastalık veya durumu bulmak ve teşhis etmek veya vücudun tedaviye ne kadar iyi tepki verdiğini görmek için bir gen ekspresyon profili kullanılabilir.

### Microarray Veri Kümeleri üzerinde istatistiksel analiz yapmanın amacı nedir?
1- En sık belirli hastalıklarla ilişkilendirilen gen dizilerindeki değişiklikleri tanımlayın

2- Belirli bir mutasyona sahip bireylerin gerçekte ne sıklıkla meme kanseri geliştirdiğini belirleyin.

3- Mikroarrayler, hücrelerde ve dokularda belirli genlerin ne ölçüde açılıp kapandığını incelemek için de kullanılabilir.

### Neyi çıkarmak istiyoruz?

Mikroarray istatistiksel analizi, önemli ölçüde değiştirilmiş gen ifadesine sahip genleri tanımlamak ister.
##
### Microarray Veri Kümesine 9 İstatistiksel Analiz Yaklaşımı
![approaches](https://user-images.githubusercontent.com/49213911/105473209-e1a95280-5cad-11eb-8e49-bf77c0cebcf7.png)
##
### T-test

T testi, farklı şekilde ifade edilen genleri tespit etmek için basit, istatistiksel temelli bir yöntemdir. Yinelenen deneylerde, hata varyansı, log oranlarından her gen için tahmin edilebilir ve her gen için standart bir t testi yapılabilir; elde edilen t istatistiği, hangi genlerin önemli ölçüde farklı şekilde ifade edildiğini belirlemek için kullanılabilir.

### BoxPlot

Kutu grafikleri, farklı dizilerdeki verilerin ölçeğinin ve dağılımının karşılaştırılabilir olup olmadığını değerlendirmenize olanak tanır. Kutuların şekil veya merkezlerindeki farklılıklar, verilerin normalleştirilmesi gerektiğini gösterir.

### Normalizasyon

Normalizasyon, ölçülen gen ekspresyon seviyelerini etkileyen bazı varyasyon kaynaklarını ortadan kaldırma işlemidir. Normalleştirme, mikrodizi veri analizinin erken aşamasında önemli bir rol oynar. Sonraki analiz sonuçları büyük ölçüde normalleşmeye bağlıdır.

Normalleştirmenin amacı, farklı şekilde ifade edilmeyen özelliklerin yoğunluklarını diziler arasında benzer hale getirmektir.
Veriler hakkında biyolojik olarak anlamlı sonuçlara varmak için numuneler arasındaki gerçek biyolojik değişkenlikten ziyade gürültüden kaynaklanan sistematik farklılıklar ortadan kaldırılmalıdır.

![beforeafterbox](https://user-images.githubusercontent.com/49213911/105473321-0c93a680-5cae-11eb-9739-bb62a5eb031b.png)

### ANOVA

Genellikle deneyci, iki hücre hattında tedavi sırasında hangi genlerin aktif olarak düzenlendiğini bilmek ister veya gruplar arasında farklı şekilde düzenlenmiş olanları seçmek için bazı kriterler ister. Bu sorular varyans analizi geleneğine (ANOVA) aittir.

Sağlık araştırmalarında, etki büyüklüğü regresyon modelleri, çok yönlü varyans analizi (ANOVA) veya çok değişkenli varyans analizi (MANOVA) gibi istatistiksel tekniklerde kullanılabilir.

### Volkan Grafiği

"Volkan grafiği", genleri biyolojik ve istatistiksel açıdan önemli boyutlara göre düzenler. Araştırmacı daha sonra, bu iki kriteri de göze alarak, takip çalışmaları için en umut verici adaylar hakkında yargılarda bulunabilir.

![volcanoplot](https://user-images.githubusercontent.com/49213911/105473441-2df49280-5cae-11eb-8009-e8878409092b.png)

### P-Değeri

P değeri, önceden belirlenmiş bir önem seviyesinden (kesme eşiği) farklı şekilde ifade edilen genleri seçmek için bir olasılık ölçüsü olarak hizmet edebilir.
Yani genler arasında bir fark olsa da, bunu bir olasılık ölçüsüne dönüştürebiliriz.

### Permütasyon Testi

Permütasyon testi, yaygın olarak uygulanabilen ve Normalden uzak dağılımlarla başa çıkan bir yaklaşımdır.
Bu yaklaşım özellikle mikrodizi çalışmaları için kullanışlıdır çünkü paralel olarak birçok gen için önem seviyelerini tahmin etmek için kolayca uyarlanabilir.
Permütasyona dayalı bir p-değeri, gerçek örneklerin tüm rastgele bölümleri arasında sözde muamele ve sözde kontrol gruplarına ait test istatistiğinin ne kadar nadir olduğunu söyler.

### Ampirik Bayes Yöntemleri

Ampirik Bayes yöntemleri, önceki dağılımın verilerden tahmin edildiği istatistiksel çıkarım prosedürleridir. Bu yaklaşım, herhangi bir veri gözlemlenmeden önce önceki dağıtımın sabitlendiği standart Bayes yöntemlerinin aksine durmaktadır.
Bayesci yaklaşımlar, tahmin edilecek parametreler hakkında varsayımlar yapar (tedavi ve kontrol gruplarındaki gen seviyeleri arasındaki farklar gibi).

### MMM (Karışım Modeli Yöntemi)

Mikrodizi verilerini analiz etmedeki önemli ve yaygın bir görev, iki deneysel koşul altında ekspresyonu değiştirilmiş genleri belirlemektir. Her deneysel koşul altında az sayıda tekrar olduğunda sorunu çözmek için karışım modeli yöntemi (MMM) adı verilen parametrik olmayan bir istatistiksel yaklaşım öneriyoruz. Spesifik olarak, sonlu normal karışım modelleri kullanarak bir t-tipi test istatistiğinin ve boş istatistiğinin dağılımlarının tahmin edilmesini öneriyoruz.

### Mikroarray verilerine istatistiksel analizi nasıl uygulayabiliriz?

1-Ham verileri okuma

2-Kalite Kontrol

3-Normalleştirme

4-Filtreleme

5-Farklı şekilde ifade edilen genlerin seçimi

6-Seçilen listelerin karşılaştırılması

7-Biyolojik Önem Analizi.


## Resources - Kaynaklar
#### https://pubmed.ncbi.nlm.nih.gov/12844246/
#### https://wiki.bits.vib.be/index.php/Analyze_your_own_microarray_data_in_R/Bioconductor#Normalization_of_microarray_data
#### https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2435252/
#### https://genomebiology.biomedcentral.com/articles/10.1186/gb-2003-4-4-210
#### https://pubmed.ncbi.nlm.nih.gov/15849016/
#### https://brb.nci.nih.gov/techreport/CIT_course_McShanePolley_May162011.pdf
#### https://www.rdocumentation.org/packages/
#### http://www.sthda.com/
#### https://www.tutorialspoint.com/
#### https://www.datanovia.com/en/blog/how-to-normalize-and-standardize-data-in-r-for-great-heatmap-visualization/
#### http://www.sthda.com/english/wiki/one-way-anova-test-in-r

##
## Buğra ATEŞ 
## https://github.com/RDSlaughter

