

# Kinetic Modeling of Human Hepatic Glucose Metabolism in Type 2 Diabetes
Mellitus Predicts Higher Risk of Hypoglycemic Events in Rigorous Insulin
Therapy*

## Kinetic Model of Human Hepatic Glucose Metabolism in T2DM

**Authors** | Matthias Koenig and Hermann-Georg Holzhuetter  
---|---  
**Corresponding Author** | Matthias Koenig   
matthias.koenig@charite.de  
Charite Berlin, Computational Systems Biochemistry, Germany  
**Keywords** | hepatic glucose metabolism; kinetic model; glucose homeostasis; liver, T2DM  
  
A major problem in the insulin therapy of patients with diabetes type 2 (T2DM)
is the increased occurrence of hypoglycemic events which, if left untreated,
may cause confusion or fainting and in severe cases seizures, coma, and even
death. To elucidate the potential contribution of the liver to hypoglycemia in
T2DM we applied a detailed kinetic model of human hepatic glucose metabolism
to simulate changes in glycolysis, gluconeogenesis, and glycogen metabolism
induced by deviations of the hormones insulin, glucagon, and epinephrine from
their normal plasma profiles. Our simulations reveal in line with experimental
and clinical data from a multitude of studies in T2DM, (i) significant changes
in the relative contribution of glycolysis, gluconeogenesis, and glycogen
metabolism to hepatic glucose production and hepatic glucose utilization; (ii)
decreased postprandial glycogen storage as well as increased glycogen
depletion in overnight fasting and short term fasting; and (iii) a shift of
the set point defining the switch between hepatic glucose production and
hepatic glucose utilization to elevated plasma glucose levels, respectively,
in T2DM relative to normal, healthy subjects. Intriguingly, our model
simulations predict a restricted gluconeogenic response of the liver under
impaired hormonal signals observed in T2DM, resulting in an increased risk of
hypoglycemia. The inability of hepatic glucose metabolism to effectively
counterbalance a decline of the blood glucose level becomes even more
pronounced in case of tightly controlled insulin treatment. Given this Janus
face mode of action of insulin, our model simulations underline the great
potential that normalization of the plasma glucagon profile may have for the
treatment of T2DM.

## Compartments

**Id** |  **Name** |  **Dimension** |  **Constant** |  **SBO** |  **GO**  
---|---|---|---|---|---  
cyto | cytosol | 3 | Y | SBO:0000290 physical compartment | GO:0005829 cytosol  
blood | blood | 3 | Y | SBO:0000290 physical compartment | GO:0005615
extracellular space  
mito | mitochondrion | 3 | Y | SBO:0000290 physical compartment | GO:0005739
mitochondrion  
mm | mitochondrial membrane | 2 | Y | SBO:0000290 physical compartment |
GO:0031966 mitochondrial membrane  
pm | plasma membrane | 2 | Y | SBO:0000290 physical compartment | GO:0005886
plasma membrane  
  
## Species

**Id** |  **Name** |  **Compartment** |  **Constant** |  **Init [mM]** |  **KEGG** |  **CHEBI** |  **UNIPROT** |  **SBO**  
---|---|---|---|---|---|---|---|---  
atp | ATP | cyto | Y | 2.8 | KEGG:C00002 | CHEBI:15422 |  | SBO:0000299
metabolite  
adp | ADP | cyto | Y | 0.8 | KEGG:C00008 | CHEBI:16761 |  | SBO:0000299
metabolite  
amp | AMP | cyto | Y | 0.16 | KEGG:C00020 | CHEBI:16027 |  | SBO:0000299
metabolite  
utp | UTP | cyto | N | 0.27 | KEGG:C00075 | CHEBI:15713 |  | SBO:0000299
metabolite  
udp | UDP | cyto | N | 0.09 | KEGG:C00015 | CHEBI:17659 |  | SBO:0000299
metabolite  
gtp | GTP | cyto | N | 0.29 | KEGG:C00044 | CHEBI:15996 |  | SBO:0000299
metabolite  
gdp | GDP | cyto | N | 0.10 | KEGG:C00035 | CHEBI:17552 |  | SBO:0000299
metabolite  
nad | NAD+ | cyto | Y | 1.22 | KEGG:C00003 | CHEBI:15846 |  | SBO:0000299
metabolite  
nadh | NADH | cyto | Y | 5.60E-004 | KEGG:C00004 | CHEBI:16908 |  |
SBO:0000299 metabolite  
p | phosphate | cyto | Y | 5 | KEGG:C00009 |  |  | SBO:0000299 metabolite  
pp | pyrophosphate | cyto | N | 0.008 | KEGG:C00013 |  |  | SBO:0000299
metabolite  
h2o | H2O | cyto | Y | 55000 | KEGG:C00001 | CHEBI:15377 |  | SBO:0000299
metabolite  
co2 | CO2 | cyto | Y | 5 | KEGG:C00011 | CHEBI:16526 |  | SBO:0000299
metabolite  
h | H+ | cyto | Y | 5.00E-008 | KEGG:C00080 | CHEBI:24636 |  | SBO:0000299
metabolite  
glc1p | glucose-1-phosphate | cyto | N | 0.012 | KEGG:C00103 | CHEBI:16077 |
| SBO:0000299 metabolite  
udpglc | UDP-glucose | cyto | N | 0.38 | KEGG:C00029 | CHEBI:18066 |  |
SBO:0000299 metabolite  
glc | glucose | cyto | N | 5 | KEGG:C00031 | CHEBI:4167 |  | SBO:0000299
metabolite  
glyglc | glycogen | cyto | N | 250 | KEGG:C00182 | CHEBI:28087 |  |
SBO:0000299 metabolite  
fru6p | fructose-6-phosphate | cyto | N | 0.05 | KEGG:C00085 | CHEBI:15946 |
| SBO:0000299 metabolite  
glc6p | glucose-6-phosphate | cyto | N | 0.12 | KEGG:C00092 | CHEBI:4170 |  |
SBO:0000299 metabolite  
fru26bp | fructose-2,6-bisphospate | cyto | N | 0.004 | KEGG:C00665 |
CHEBI:28602 |  | SBO:0000299 metabolite  
fru16bp | fructose-1,6-bisphospate | cyto | N | 0.02 | KEGG:C00354 |
CHEBI:16905 |  | SBO:0000299 metabolite  
dhap | dihydroxyacetone phosphate | cyto | N | 0.03 | KEGG:C00111 |
CHEBI:16108 |  | SBO:0000299 metabolite  
grap | glyceraldehyde 3-phosphate | cyto | N | 0.1 | KEGG:C00118 | CHEBI:29052
|  | SBO:0000299 metabolite  
pg3 | 3-phosphoglycerate | cyto | N | 0.27 | KEGG:C00197 | CHEBI:17794 |  |
SBO:0000299 metabolite  
bpg13 | 1,3-bisphospho-glycerate | cyto | N | 0.3 | KEGG:C00236 | CHEBI:16001
|  | SBO:0000299 metabolite  
pep | phosphoenolpyruvate | cyto | N | 0.15 | KEGG:C00074 | CHEBI:44897 |  |
SBO:0000299 metabolite  
pg2 | 2-phosphoglycerate | cyto | N | 0.03 | KEGG:C00631 | CHEBI:17835 |  |
SBO:0000299 metabolite  
oaa | oxaloacetate | cyto | N | 0.01 | KEGG:C00036 | CHEBI:30744 |  |
SBO:0000299 metabolite  
pyr | pyruvate | cyto | N | 0.1 | KEGG:C00022 | CHEBI:32816 |  | SBO:0000299
metabolite  
glc_blood | glucose | blood | Y | 5 | KEGG:C00031 | CHEBI:4167 |  |
SBO:0000299 metabolite  
lac | lactate | cyto | N | 0.5 | KEGG:C00186 | CHEBI:422 |  | SBO:0000299
metabolite  
p_mito | phosphate | mito | Y | 5 | KEGG:C00009 |  |  | SBO:0000299 metabolite  
oaa_mito | oxaloacetate | mito | N | 0.01 | KEGG:C00036 | CHEBI:30744 |  |
SBO:0000299 metabolite  
lac_blood | lactate | blood | Y | 1.2 | KEGG:C00186 | CHEBI:422 |  |
SBO:0000299 metabolite  
co2_mito | CO2 | mito | Y | 5 | KEGG:C00011 | CHEBI:16526 |  | SBO:0000299
metabolite  
pyr_mito | pyruvate | mito | N | 0.1 | KEGG:C00022 | CHEBI:32816 |  |
SBO:0000299 metabolite  
cit_mito | citrate | mito | Y | 0.32 | KEGG:C00158 | CHEBI:30769 |  |
SBO:0000299 metabolite  
pep_mito | pep | mito | N | 0.15 | KEGG:C00074 | CHEBI:44897 |  | SBO:0000299
metabolite  
acoa_mito | acetyl-coenzyme A | mito | Y | 0.04 | KEGG:C00024 | CHEBI:15351 |
| SBO:0000299 metabolite  
gtp_mito | GTP | mito | N | 0.29 | KEGG:C00044 | CHEBI:15996 |  | SBO:0000299
metabolite  
gdp_mito | GDP | mito | N | 0.10 | KEGG:C00035 | CHEBI:17552 |  | SBO:0000299
metabolite  
atp_mito | ATP | mito | Y | 2.8 | KEGG:C00002 | CHEBI:15422 |  | SBO:0000299
metabolite  
adp_mito | ADP | mito | Y | 0.8 | KEGG:C00008 | CHEBI:16761 |  | SBO:0000299
metabolite  
nad_mito | NAD+ | mito | Y | 0.98 | KEGG:C00003 | CHEBI:15846 |  | SBO:0000299
metabolite  
h_mito | H+ | mito | Y | 1.00E-008 | KEGG:C00011 | CHEBI:24636 |  |
SBO:0000299 metabolite  
coa_mito | coenzymeA | mito | Y | 0.055 | KEGG:C00010 | CHEBI:15346 |  |
SBO:0000299 metabolite  
nadh_mito | NADH | mito | Y | 0.24 | KEGG:C00004 | CHEBI:16908 |  |
SBO:0000299 metabolite  
epinephrine_blood | epinephrine | blood | N | 206.11 | KEGG:C00547 |
CHEBI:18357 |  | SBO:0000299 metabolite  
glucagon_blood | glucagon | blood | N | 4.36E-008 | KEGG:C01501 |  |
UNIPROT:P01275 | SBO:0000299 metabolite  
insulin_blood | insulin | blood | N | 7.61E-008 | KEGG:C00723 |  |
UNIPROT:P01308 | SBO:0000299 metabolite  
h20_mito | H2O | mito | Y | 55000 | KEGG:C00080 | CHEBI:15377 |  | SBO:0000299
metabolite  
  
## Reactions

**Id** |  **Name** |  **Compartment** |  **Irreversible** |  **Vmax [µmol/kg/min]** |  **EC** |  **KEGG** |  **UNIPROT** |  **SBO**  
---|---|---|---|---|---|---|---|---  
GLUT2 | GLUT2 glucose transporter (facilitated diffusion) | pm | N | 420 |  |
| UNIPROT:P11168 | SBO:0000284 transporter  
GK | Glucokinase, hexokinase IV | cyto | Y | 25.2 | EC:2.7.1.2 | KEGG:R00299 |
UNIPROT:P35557 | SBO:0000014 enzyme  
G6PASE | Glucose-6-phosphatase | cyto | Y | 18.9 | EC:3.1.3.9 | KEGG:R00303 |
UNIPROT:P35575 | SBO:0000014 enzyme  
GPI | Glucose-6-phosphate isomerase | cyto | N | 420 | EC:5.3.1.9 |
KEGG:R00771 | UNIPROT:P06744 | SBO:0000014 enzyme  
G16PI | glucose-1-phosphate 1,6-phosphomutase | cyto | N | 100 | EC:5.4.2.2 |
KEGG:R00959 | UNIPROT:P36871, UNIPROT:Q96G03 | SBO:0000014 enzyme  
UPGASE | UTP:Glucose-1-phosphate uridylyltransferase | cyto | N | 80 |
EC:2.7.7.9 | KEGG:R00289 | UNIPROT:Q16851 | SBO:0000014 enzyme  
PPASE | Pyrophosphate phosphohydrolase | cyto | Y | 2.4 | EC:3.6.1.1 |
KEGG:R00004 | UNIPROT:Q15181 | SBO:0000014 enzyme  
GS | Glycogen synthase | cyto | Y | 13.2 |  |  | UNIPROT:P54840 | SBO:0000014
enzyme  
GP | Glycogen phosphorylase | cyto | N | 6.8 |  |  | UNIPROT:P06737 |
SBO:0000014 enzyme  
NTKGTP | Nucleosid diphosphate kinase (GTP) | cyto | N | 0 | EC:2.7.4.6 |
KEGG:R00330 |  | SBO:0000014 enzyme  
NTKUTP | Nucleosid diphosphate kinase (UTP) | cyto | N | 2940 | EC:2.7.4.6 |
KEGG:R00156 |  | SBO:0000014 enzyme  
AK | Adenylat kinase | cyto | N | 0 | EC:2.7.4.3 | KEGG:R00127 |  |
SBO:0000014 enzyme  
PFK2 | Phosphofructo kinase 2 | cyto | Y | 0.0042 | EC:2.7.1.105 | KEGG:R02732
| UNIPROT:P16118 | SBO:0000014 enzyme  
FBP2 | Fructose-2,6-bisphosphatase | cyto | Y | 0.126 | EC:3.1.3.46 |
KEGG:R02731 | UNIPROT:P16118 | SBO:0000014 enzyme  
PFK1 | Phosphofructo kinase 1 | cyto | Y | 7.182 | EC:2.7.1.11 | KEGG:R00756 |
UNIPROT:P17858 | SBO:0000014 enzyme  
FBP1 | Fructose-1,6-bisphosphatase | cyto | Y | 4.326 | EC:3.1.3.11 |
KEGG:R00762 | UNIPROT:O00757, UNIPROT:P09467 | SBO:0000014 enzyme  
TPI | Triosephosphate isomerase | cyto | N | 420 | EC:5.3.1.1 | KEGG:R01015 |
UNIPROT:P60174 | SBO:0000014 enzyme  
ALD | Aldolase | cyto | N | 420 | EC:4.1.2.13 | KEGG:R01068 | UNIPROT:P05062 |
SBO:0000014 enzyme  
PGK | Phosphoglycerate kinase | cyto | N | 420 | EC:2.7.2.3 | KEGG:R01512 |
UNIPROT:P00558 | SBO:0000014 enzyme  
GAPDH | Glyceraldehydephosphate dehydrogenase | cyto | N | 420 | EC:1.2.1.12 |
KEGG:R01061 | UNIPROT:P04406 | SBO:0000014 enzyme  
EN | Enolase | cyto | N | 35.994 | EC:4.2.1.11 | KEGG:R00658 | UNIPROT:P06733,
UNIPROT:P09104, UNIPROT:P13929 | SBO:0000014 enzyme  
PGAM | 3-Phosphoglycerate mutase | cyto | N | 420 | EC:5.4.2.1 | KEGG:R01518 |
UNIPROT:P18669 | SBO:0000014 enzyme  
PEPCK | Phosphoenolpyruvate carboxykinase | cyto | N | 0 | EC:4.1.1.32 |
KEGG:R00431 | UNIPROT:P35558 | SBO:0000014 enzyme  
PK | Pyruvate kinase | cyto | Y | 46.2 | EC:2.7.1.40 | KEGG:R00200 |
UNIPROT:P30613 | SBO:0000014 enzyme  
PC | Pyruvate Carboxylase | mito | Y | 168 | EC:6.4.1.1 | KEGG:R00344 |
UNIPROT:P11498 | SBO:0000014 enzyme  
PEPCK_mito | Phosphoenolpyruvate carboxykinase | mito | N | 546 | EC:4.1.1.32
| KEGG:R00431 | UNIPROT:Q16822 | SBO:0000014 enzyme  
LACT | Lactate transporter | pm | N | 5.418 |  |  |  | SBO:0000284 transporter  
LDH | Lactate dehydrogenase | cyto | N | 12.6 | EC:1.1.1.27 | -KEGG:R00703 |
UNIPROT:P00338, UNIPROT:P07195, UNIPROT:P07864 | SBO:0000014 enzyme  
PEPT | PEP transporter | mm | N | 33.6 |  |  |  | SBO:0000284 transporter  
PYRT | Pyruvate transporter | mm | N | 42 |  |  |  | SBO:0000284 transporter  
CS | Citrate synthase | mito | N | 4.2 | EC:2.3.3.1 | -KEGG:R00351 |
UNIPROT:O75390 | SBO:0000014 enzyme  
PDH | Pyruvate dehydrogenase | mito | Y | 13.44 | EC:1.2.4.1 | KEGG:R00209 |
UNIPROT:P08559, UNIPROT:P11177, UNIPROT:P10515, UNIPROT:P09622, O00330 |
SBO:0000014 enzyme  
ACOAFLX | Acetyl-CoA flux | mito | N | 0 |  |  |  | SBO:0000014 enzyme  
VCITFLX | Citrate flux | mito | N | 0 |  |  |  | SBO:0000014 enzyme  
NDK_mito | Nucleosid diphosphate kinase (GTP) | mito | N | 420 | EC:2.7.4.6 |
KEGG:R00330 |  | SBO:0000014 enzyme  
OAAFLX | Oxalacetate flux | mito | N | 0 |  |  |  | SBO:0000014 enzyme

