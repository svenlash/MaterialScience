### Расчёт TPSA и Labute ASA для ciguatoxin
**Результат расчёта:** [посмотреть на GitHub Actions](https://github.com/svenlash/MaterialScience/actions/runs/35005620351/job/104504509682)![Run TPSA](https://github.com/svenlash/MaterialScience/actions/workflows/run.yml/badge.svg)

## Базы данных

<table border="0" cellspacing="0" cellpadding="0" width="100%">
<tr>
<td valign="top" width="50%">

<h3>🧪</h3>

| № | База данных | Сайт |
|---|-------------|------|
| 1 | PubChem | [pubchem.ncbi.nlm.nih.gov](https://pubchem.ncbi.nlm.nih.gov/) |
| 2 | ChemSpider | [chemspider.com](http://www.chemspider.com/) |
| 3 | Chemical Synthesis | [chemsynthesis.com](https://www.chemsynthesis.com/) |
| 4 | CAS | [commonchemistry.cas.org](https://commonchemistry.cas.org/) |
| 5 | COD | [crystallography.net](http://www.crystallography.net/cod/) |
| 6 | MINCRYST | [database.iem.ac.ru](http://database.iem.ac.ru/mincryst/rus/index.php) |
| 7 | ChemSub Online | [chemsub.online.fr](http://chemsub.online.fr/) |
| 8 | MassBank | [massbank.jp](http://www.massbank.jp/) |
| 9 | Wiley | [onlinelibrary.wiley.com](https://onlinelibrary.wiley.com/library-info/products/databases) |
| 10 | NIST | [chemdata.nist.gov](https://chemdata.nist.gov/) |

</td>
<td valign="top" width="50%">

<h3>🧬</h3>

| № | База данных | Сайт |
|---|-------------|------|
| 1 | RCSB PDB | [rcsb.org](https://www.rcsb.org/) |
| 2 | Nucleic Acid Database | [ndbserver.rutgers.edu](http://ndbserver.rutgers.edu/) |
| 3 | DrugBank | [go.drugbank.com](https://go.drugbank.com/) |
| 4 | ChEMBL | [ebi.ac.uk/chembl](https://www.ebi.ac.uk/chembl/) |
| 5 | BMRB | [bmrb.wisc.edu](http://www.bmrb.wisc.edu/) |
| 6 | SMPDB | [smpdb.ca](https://smpdb.ca/) |
| 7 | CTD | [ctdbase.org](https://ctdbase.org/) |
| 8 | EnviPath | [envipath.org](https://envipath.org/) |
| 9 | T3DB | [t3db.ca](http://www.t3db.ca/) |
| 10 | BindingDB | [bindingdb.org](http://www.bindingdb.org/bind/index.jsp) |
| 11 | GenomeNet | [genome.jp](https://www.genome.jp/) |
| 12 | MCDB | [mcdb.ca](https://mcdb.ca/) |

</td>
</tr>
</table>

<table border="0" cellspacing="0" cellpadding="0" width="100%">
<tr>
<td valign="top" width="50%">

<h3>Редакторы</h3>

| № | Программа | Сайт |
|---|-----------|------|
| 1 | MolView | [molview.org](https://molview.org/) |
| 2 | Jmol | [jmol.sourceforge.net](https://jmol.sourceforge.net/) |
| 3 | Molsoft | [molsoft.com](https://www.molsoft.com/) |
| 4 | JSME | [jsme-editor.github.io](https://jsme-editor.github.io/) |
| 5 | Mendeleev-plus | [mendeleevplus.com](https://mendeleevplus.com/) |
| 6 | LEA3D | [leahcim.net](http://leahcim.net/lea3d/) |
| 7 | MOLINSPIR | [molinspiration.com](https://www.molinspiration.com/) |
| 8 | CheMagic | [chemagic.org](https://chemagic.org/) |

</td>
<td valign="top" width="50%">

<h3>Визуализаторы</h3>

| № | Программа | Сайт |
|---|-----------|------|
| 9 | MaSK | [mask.bmrb.wisc.edu](https://mask.bmrb.wisc.edu/) |
| 10 | Cheminfo | [cheminfo.org](https://cheminfo.org/) |
| 11 | BKChem | [bkchem.zirael.org](http://bkchem.zirael.org/) |
| 12 | Avogadro | [avogadro.cc](https://avogadro.cc/) |
| 13 | Gabedit | [gabedit.sourceforge.net](http://gabedit.sourceforge.net/) |
| 14 | Ascalaph | [ascalaph.agate.net](http://www.ascalaph.agate.net/) |
| 15 | YASARA | [yasara.org](https://www.yasara.org/) |

</td>
</tr>
</table>
# 📁 Форматы химических файлов

## Краткое сравнение

| Формат | Что хранит | Молекул в файле | Для чего |
|--------|------------|-----------------|----------|
| **MOL** | 1 молекула | 1 | Малые молекулы |
| **SDF** | Молекулы + данные | Много | Базы данных |
| **PDB** | Макромолекула | 1 | Белки, ДНК |
| **CSV** | Таблица | — | Данные для Excel |
| **SMILES** | Строка | 1 | Быстрая запись |

---

## 🔹 MOL — одна молекула

**Что содержит:**
- Атомы (координаты, тип)
- Связи (порядок)
- Заряды, изотопы, стереохимию

**Версии:**

| Версия | Макс. атомов | Особенности |
|--------|--------------|-------------|
| **V2000** | 999 | Старый, универсальный |
| **V3000** | ~1 млрд | Новый, для больших молекул |

**Пример:**
```
  Mrv1810 04281710402D

  5  4  0  0  0  0  0  0  0  0999 V2000
    1.3300   -1.3300    0.0000 P ...
    1.3300   -2.6600    0.0000 O ...
  ...
  1  3  1  0  0  0  0
  1  5  1  0  0  0  0
M  END
```

**Когда использовать:** одна молекула, совместимость со всеми программами.

---

## 🔹 SDF — много молекул + данные

**Что содержит:**
- Несколько MOL-блоков
- Свойства (CAS, TPSA, LogP, MMFF94_Energy)
- Разделитель `$$$$`

**Структура:**
```
Молекула 1 (MOL)
> <Property1>
значение
$$$$
Молекула 2 (MOL)
...
$$$$
```

**Где используется:**
- PubChem, ChEBI, DrugBank, ZINC
- RDKit, OpenBabel, DataWarrior

**Когда использовать:** базы данных, анализ множества молекул, обмен данными.

---

## 🔹 PDB — макромолекулы

**Что содержит:**
- 3D-координаты белков, ДНК, РНК
- Лиганды (HETATM)
- Вторичную структуру (HELIX, SHEET)
- Метаданные (метод, разрешение)

**Пример:**
```
HEADER    HYDROLASE
ATOM      1  N   ALA A   1   10.000 20.000 30.000
HETATM 1000  C1  BCD A 500   50.000 60.000 70.000
END
```

**Где используется:**
- RCSB PDB, PyMOL, Chimera, VMD

**Когда использовать:** структуры белков, молекулярная динамика, докинг.

---

## 🔹 SMILES — строка

**Что содержит:** текстовую запись молекулы.

**Пример:**
- Бензол: `c1ccccc1`
- Этанол: `CCO`
- Аспирин: `CC(=O)Oc1ccccc1C(=O)O`

**Когда использовать:** быстрая запись, поиск, базы данных.

---

## 🔹 CSV — таблица

**Что содержит:** данные в виде таблицы (разделитель — запятая).

**Пример:**
```
Название,Формула,MW,TPSA
Антрацен,C14H10,178.23,0.00
```

**Когда использовать:** Excel, анализ, отчёты.

---

## 🔄 Конвертация форматов

| Из | В | Инструмент |
|----|---|-----------|
| MOL | SDF | RDKit, OpenBabel |
| SDF | CSV | RDKit, OpenBabel |
| SDF | PDB | OpenBabel |
| PDB | MOL | OpenBabel, RDKit |
| SMILES | MOL | RDKit, OpenBabel |

**RDKit (Python):**
```python
from rdkit import Chem

mol = Chem.MolFromMolFile('input.mol')          # MOL → mol
Chem.MolToMolFile(mol, 'output.mol')            # mol → MOL
Chem.MolToSmiles(mol)                           # mol → SMILES
```

**OpenBabel (командная строка):**
```bash
obabel input.sdf -O output.csv
obabel input.pdb -O output.mol
```

---

## 🧰 Программы для просмотра

| Формат | Программа |
|--------|-----------|
| MOL, SDF | Avogadro, RDKit, MolView |
| PDB | PyMOL, Chimera, VMD |
| SMILES | RDKit, ChemDraw |
| CSV | Excel, Google Sheets |

---

## 📌 Что запомнить

| Формат | Ключевое |
|--------|----------|
| **MOL** | Одна молекула |
| **SDF** | MOL + данные + `$$$$` |
| **PDB** | Белки и макромолекулы |
| **SMILES** | Строка |
| **CSV** | Таблица |

**SDF = MOL + данные.**
**PDB — для биологов, SDF — для химиков.**
