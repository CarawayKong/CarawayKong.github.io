---
title: qPCR
description: 基础实验
date: 2025-03-28 00:00:00+0000
image: 
categories:
    - Protocol
tags:
    - 
weight: 1       # You can add weight to some posts to override the default sorting (date descending)
---

# 实时荧光定量PCR实验方案  

---

## RNA提取

---

**组织来源**  
准备材料：Trizol，氯仿，DEPC 水，异丙醇，无水乙醇
1. 组织匀浆器底座 -20℃ 提前预冷。
2. 离心机提前打开，4℃ 预冷。根据样本量，标记离心管，每管加入 1 ml Trizol。<mark>（有毒，通风橱中操作）</mark>
3. 每管加入 2 颗钢珠，在组织匀浆器中 65 Hz 研磨 120 s，涡旋混匀，静置 10 min。
4. 每管加入 200 μl氯仿，在通风橱中涡旋混匀 10 s，室温静置 10 min。
5. 在 4℃ 下 16000 G 离心 20 min，弃下层沉淀，吸取上清。
6. 按照 1 ∶ 2 或  1 ∶ 1 （源体积 ∶ 异丙醇）的比例加入异丙醇。盖上盖子，上下颠倒 10 次（上下为一次）。
7. -20℃ 沉淀，大于 2 h，离心机 4℃ 预冷。
8. 在 4℃ 下 16000 G 离心 20 min，弃上清。沿沉淀的另一侧倒出。
9. 用含 75% 酒精的 DEPC 水清洗沉淀，每管 1ml，涡旋 3~4 次。
10. 在 4℃ 下 16000 G 离心 20 min，弃上清，在纸上倒置晾干 10~20 min。
11. 加 20 μl 冰浴的 DEPC 水，吹打，使沉淀溶解，置于冰上。  
    <mark>RNA 提出后一定要放冰上，不能放室温。</mark>
12. 测浓度后，可立即用于逆转录，也可液氮速冻存于 -80℃。
---

**细胞来源**  
准备材料与组织提取相同  
1. 在六孔板中贴壁生长的细胞，去掉上清，用 PBS 轻轻洗 2 遍后，每孔加 500 μl Trizol，多次吹打后将液体转移至 1.5 ml 离心管，涡旋混匀，静置 10 min。  
2. 后续步骤与「组织来源」相同，从第 4 步开始。

---

## 逆转录合成 cDNA 第一链  
**使用 翌圣 Hifair® Ⅲ 1st Strand cDNA Synthesis SuperMix for qPCR 试剂盒**  

试剂盒组分  
+ RNase-free H<sub>2</sub>O
+ 5× gDNA digester Mix
+ 4× Hifair® Ⅲ SuperMix plus   
注：4× Hifair® Ⅲ SuperMix plus 含有 gDNA digester 抑制剂。

1. 残留基因组 DNA 去除   
    + 在 RNase free 离心管中配制如下混合液，用移液器轻轻吹打混匀。42℃ 孵育 2 min。
  
    |组分|使用量|
    |:---:|:---:|
    |Total RNA|1 μg|
    |5× gDNA digester Mix|3 μl|
    |RNase-free H<sub>2</sub>O|To 15 μl|

    + <mark>配制母液时需考虑损失体积，单次移液，体积 × 1.04；两次移液，体积 × 1.08</mark>

2. 逆转录反应体系配制（20 μl 体系）  
   + 在第 1 步的反应管中直接加入 5 μl 4× Hifair® Ⅲ SuperMix plus，用移液器轻轻吹打混匀。
3. 逆转录程序设置
    |温度|时间|
    |:---:|:---:|
    |25℃|5 min|
    |55℃|15 min|
    |85℃|5 min|

4. 可立即用于 qPCR 也可分装后液氮速冻，存于 -80℃。

---

## qPCR
**使用翌圣 Hieff UNICON® Universal Blue qPCR SYBR Green Master Mix 试剂盒** 

准备的材料：试剂盒、cDNA原液、qPCR 96 孔板、封板膜

1. 于超净台内在冰上配置反应体系<mark>（96 孔板可卡在底座上，底座置于冰上）</mark>。  
  
|组分|体积 (μl)|体积 (μl)|终浓度|
|:---:|:---:|:---:|:---:|
|Hieff UNICON® Universal Blue qPCR SYBR Green Master Mix|25|10|1×|
|Forward Primer (10 μM)|1|0.4|0.2 μM|
|Reverse Primer (10 μM)1|1|0.4|0.2 μM|
|模板 DNA|X|X|-|
|无菌超纯水|to 50|to 20|-|  

+ cDNA 原液体积一般不超过反应总体积的 1/10
+ 先将体系配好<mark>（留好余量，例如配每孔 20 μl 体系，加 19 μl）</mark>并加入 96 孔板，再点加 cDNA 在孔板上缘，点板完成后用膜封板，再使用离心机甩板。
+ 定量实验需要至少 3 个 生物学重复
+ 需要设置内参
  
2. 上机  

    标准程序  

<table>
    <tr>
        <td align="center">循环步骤</td>
        <td align="center">温度</td>
        <td align="center">时间</td>
        <td align="center">循环数</td>
    </tr>
    <tr>
        <td align="center">预变性</td>
        <td align="center">95℃</td>
        <td align="center">2 min</td>
        <td align="center">1</td>
    </tr>
    <tr>
        <td align="center">变性</td>
        <td align="center">95℃</td>
        <td align="center">10 sec</td>
        <td align="center" rowspan=2>40</td>
    </tr>
    <tr>
        <td align="center">退火/延伸</td>
        <td align="center">60℃</td>
        <td align="center">30 sec</td>
    </tr>
    <tr>
        <td align="center">熔解曲线阶段</td>
        <td align="center" colspan=2>仪器默认设置</td>
        <td align="center">1</td>
    </tr>
</table>

3. 结果分析  
   + 扩增曲线：标准扩增曲线为S型。  
      + Ct值落在 20~30 之间时，定量分析最准确； 
      + Ct值小于 10，需要将稀释模板后，重新进行实验； 
      + Ct值介于 30~35 之间时，需要提高模板浓度，或者增大反应体系的体积，以提高扩增效率，保证结果分析的准确性； 
      + Ct值大于 35 时，检测结果无法定量分析基因的表达量，但可用于定性分析。 
    + 熔解曲线： 
      + 熔解曲线单峰，表明反应特异性好可以进行定量结果分析；若熔解曲线出现双峰或者多峰，则不能进行定量分析。 
      + 熔解曲线出现双峰，需要通过 DNA 琼脂糖凝胶电泳判断非目标峰是引物二聚体还是非特异性扩增。 
      + 如果是引物二聚体，建议降低引物浓度，或者重新设计扩增效率高的引物。 
      + 如果是非特异性扩增，请提高退火温度，或者重新设计更高特异性的引物。
4. 引物设计指南
   + 推荐引物长度 25 bp 左右。扩增产物长度 150 bp 为佳，可以在 100 bp~300 bp 内选择。 
   + 正向引物和反向引物的 Tm 值相差不宜超过 2℃。引物 Tm 值 60℃~65℃ 为佳。 
   + 引物碱基分布要均匀，避免出现连续的 4 个相同碱基，GC 含量控制在 50% 左右。3' 端最后一个碱基最好为 G 或 C。 
   + 引物内部或者正反两条引物间最好避免出现有3个碱基以上的互补序列。 
   + 引物特异性需要用 NCBI BLAST 程序进行核对。避免引物 3' 端有 2 个碱基以上的非特异性互补。 
   + 设计完成的引物需要进行扩增效率的检测，只有具备相同扩增效率的引物才可用于定量比较分析。 