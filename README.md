# Messenger bags: online and in-person preferences

The same 122 people rated the same 20 messenger bags twice, first online and then in person. Size showed the clearest reversal. Holding price and the other features constant, participants rated a large bag 0.27 points higher than a small one online and 0.31 points lower in person. The ratings used a five-point purchase-intent scale. Since everyone rated the bags in the same order, some of the shift could come from seeing them a second time.

I used conjoint analysis to estimate how much exterior design, size, price, a strap pad, a bottle pocket and interior compartments contributed to each person's rating. I then used those estimates to compare 384 combinations of features and prices. In the simulation, a participant buys a bag if its predicted rating reaches 3.5 out of 5.

| Ratings used | Highest-revenue single bag | Price | Predicted buyers out of 122 | Estimated revenue |
| --- | --- | ---: | ---: | ---: |
| Online | Large, black | $160 | 84 | $13,440 |
| In person | Small, black | $180 | 58 | $10,440 |

Both bags have a strap pad, a bottle pocket and a padded laptop compartment. Offering two designs changed the online result. The best pair combined a large black bag at $180 with a small blue bag at $120. With each person choosing at most one bag, the pair attracted 92 predicted buyers and earned $14,820 in the simulation.

## Reading the project

- `output/report.pdf` explains the study design, the preference estimates and the product choices.
- `output/results.pdf` collects the regression tables and figures. Individual tables and plots are also in `output/tables/` and `output/plots/`.
- `code/code.ipynb` contains the analysis, from matching ratings to bag profiles through the two-bag search.
- `input/` contains the three original CSVs. Each row of the design file describes one bag. In each ratings file, rows are participants and columns follow the bag order in the design file.

To rerun the notebook, use Jupyter with NumPy, pandas, statsmodels, Matplotlib and seaborn installed. The notebook reads the CSVs by filename. With the kernel starting in `code/`, run `%cd ../input` in a cell before executing the analysis.

Vadim Volozhenin