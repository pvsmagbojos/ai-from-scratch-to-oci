# AI Learning Roadmap — Master Checklist

## Phase 0 — Learning Environment and Foundations

### 0.1 Development Environment
- [ ] Install Python 3.
- [ ] Understand what the Python interpreter is.
- [ ] Understand Python versions and compatibility.
- [ ] Install Visual Studio Code.
- [ ] Install the Python extension for VS Code.
- [ ] Install JupyterLab / Jupyter Notebook.
- [ ] Understand what a Jupyter kernel is.
- [ ] Understand notebooks versus Python scripts.
- [ ] Learn how to run individual notebook cells.
- [ ] Learn Markdown cells in Jupyter.
- [ ] Learn how notebook state works.
- [ ] Learn why running notebook cells out of order can cause problems.
- [ ] Learn how to restart and clear a notebook kernel.
- [ ] Learn terminal / command-line basics.
- [ ] Learn basic Windows PowerShell or shell commands.
- [ ] Learn `pip`.
- [ ] Learn virtual environments with `venv`.
- [ ] Learn dependency files such as `requirements.txt`.
- [ ] Learn the purpose of Conda environments.
- [ ] Install and configure Git.
- [ ] Learn basic Git workflows.
  - [ ] `git init`
  - [ ] `git clone`
  - [ ] `git status`
  - [ ] `git add`
  - [ ] `git commit`
  - [ ] `git pull`
  - [ ] `git push`
  - [ ] branches
  - [ ] merging
- [ ] Create a dedicated Git repository for AI exercises and projects.
- [x] Create a consistent folder structure for course exercises.
- [ ] Learn how environment variables work.
- [ ] Learn why API keys and credentials must not be committed to Git.

### 0.2 Computer Science Foundations
- [ ] Understand bits, bytes, KB, MB, GB, and memory.
- [ ] Understand CPU versus GPU computation.
- [ ] Understand processes and threads at a basic level.
- [ ] Understand files, directories, paths, and file permissions.
- [ ] Understand client/server architecture.
- [ ] Understand HTTP.
- [ ] Understand HTTP methods.
  - [ ] GET
  - [ ] POST
  - [ ] PUT/PATCH
  - [ ] DELETE
- [ ] Understand HTTP status codes.
- [ ] Understand JSON.
- [ ] Understand REST APIs.
- [ ] Understand request headers and authentication.
- [ ] Understand synchronous versus asynchronous operations.
- [ ] Understand latency versus throughput.
- [ ] Understand batch processing versus real-time processing.
- [ ] Understand databases at a high level.
- [ ] Understand relational versus non-relational data.
- [ ] Understand basic SQL.

### 0.3 AI Vocabulary
- [ ] Define artificial intelligence.
- [ ] Define machine learning.
- [ ] Define deep learning.
- [ ] Define generative AI.
- [ ] Define an AI model.
- [ ] Define training.
- [ ] Define inference.
- [ ] Define parameters.
- [ ] Define hyperparameters.
- [ ] Define features.
- [ ] Define labels.
- [ ] Define datasets.
- [ ] Distinguish supervised, unsupervised, semi-supervised, and reinforcement learning.
- [ ] Distinguish discriminative and generative models.
- [ ] Understand narrow AI versus artificial general intelligence.
- [ ] Understand deterministic software versus probabilistic models.
- [ ] Understand that modern AI systems are usually combinations of models, software, data systems, infrastructure, and business logic.

### Phase 0 Exit Criteria
- [ ] Create and run a Python script.
- [ ] Create and run a Jupyter notebook.
- [ ] Install a Python dependency in an isolated environment.
- [ ] Call a simple REST API from Python.
- [ ] Parse a JSON response.
- [ ] Commit the work to Git.
- [ ] Explain the difference between AI, ML, deep learning, generative AI, training, and inference without notes.

---

# Phase 1 — Python for Data Science and AI

## 1.1 Python Fundamentals
- [ ] Variables.
- [ ] Primitive data types.
  - [ ] integers
  - [ ] floats
  - [ ] strings
  - [ ] booleans
  - [ ] `None`
- [ ] Operators.
- [ ] String manipulation.
- [ ] Lists.
- [ ] Tuples.
- [ ] Dictionaries.
- [ ] Sets.
- [ ] Indexing.
- [ ] Slicing.
- [ ] Conditional statements.
- [ ] `for` loops.
- [ ] `while` loops.
- [ ] Functions.
- [ ] Function parameters.
- [ ] Return values.
- [ ] Default parameters.
- [ ] Keyword arguments.
- [ ] Scope.
- [ ] List comprehensions.
- [ ] Dictionary comprehensions.
- [ ] Exceptions.
- [ ] Reading and writing files.
- [ ] Importing modules.
- [ ] Creating modules.
- [ ] Creating packages.

## 1.2 Intermediate Python
- [ ] Classes and objects.
- [ ] Constructors.
- [ ] Instance attributes.
- [ ] Methods.
- [ ] Inheritance.
- [ ] Composition.
- [ ] Dataclasses.
- [ ] Type annotations.
- [ ] Generics at a practical level.
- [ ] Iterators.
- [ ] Generators.
- [ ] Decorators.
- [ ] Context managers.
- [ ] Lambda functions.
- [ ] `map`, `filter`, and `reduce`.
- [ ] Understand mutable versus immutable objects.
- [ ] Understand references and copying.
- [ ] Understand shallow versus deep copies.
- [ ] Understand Python package management.
- [ ] Learn basic Python debugging.
- [ ] Learn logging.
- [ ] Learn unit testing with `pytest`.

## 1.3 NumPy
- [ ] Understand why NumPy is used in numerical computing.
- [ ] Create NumPy arrays.
- [ ] Understand array shapes.
- [ ] Understand dimensions and axes.
- [ ] Index arrays.
- [ ] Slice arrays.
- [ ] Reshape arrays.
- [ ] Understand broadcasting.
- [ ] Perform element-wise operations.
- [ ] Perform matrix operations.
- [ ] Calculate aggregates.
- [ ] Use boolean masks.
- [ ] Understand vectorization.
- [ ] Compare vectorized operations against Python loops.
- [ ] Understand NumPy random-number generation.
- [ ] Understand reproducibility and random seeds.

## 1.4 pandas
- [ ] Understand Series.
- [ ] Understand DataFrames.
- [ ] Load CSV data.
- [ ] Load JSON data.
- [ ] Load Excel data.
- [ ] Inspect datasets.
- [ ] Select columns.
- [ ] Filter rows.
- [ ] Sort data.
- [ ] Handle missing values.
- [ ] Handle duplicates.
- [ ] Convert data types.
- [ ] Manipulate strings.
- [ ] Work with dates and times.
- [ ] Group and aggregate data.
- [ ] Join datasets.
- [ ] Merge datasets.
- [ ] Pivot datasets.
- [ ] Apply transformations.
- [ ] Identify inefficient row-by-row operations.
- [ ] Prefer vectorized operations where appropriate.

## 1.5 Data Visualization
- [ ] Learn Matplotlib.
- [ ] Create line charts.
- [ ] Create bar charts.
- [ ] Create scatter plots.
- [ ] Create histograms.
- [ ] Create box plots.
- [ ] Visualize distributions.
- [ ] Visualize correlations.
- [ ] Choose appropriate chart types.
- [ ] Avoid misleading visualizations.
- [ ] Create readable labels, legends, and axes.

### Phase 1 Project
- [ ] Obtain a real-world dataset.
- [ ] Load the dataset with pandas.
- [ ] Clean the dataset.
- [ ] Explore the dataset.
- [ ] Calculate descriptive statistics.
- [ ] Produce useful visualizations.
- [ ] Document findings in Jupyter.
- [ ] Commit the project to Git.

### Phase 1 Exit Criteria
- [ ] Manipulate a dataset without step-by-step instructions.
- [ ] Explain NumPy arrays and pandas DataFrames.
- [ ] Write reusable Python functions.
- [ ] Debug common Python errors.
- [ ] Build a complete exploratory-data-analysis notebook.

---

# Phase 2 — Mathematics for AI

## 2.1 Arithmetic and Algebra Refresh
- [ ] Fractions.
- [ ] Percentages.
- [ ] Exponents.
- [ ] Roots.
- [ ] Logarithms.
- [ ] Scientific notation.
- [ ] Variables.
- [ ] Equations.
- [ ] Functions.
- [ ] Function notation.
- [ ] Linear functions.
- [ ] Polynomial functions.
- [ ] Exponential functions.
- [ ] Logarithmic functions.
- [ ] Systems of equations.

## 2.2 Linear Algebra
- [ ] Scalars.
- [ ] Vectors.
- [ ] Matrices.
- [ ] Tensors.
- [ ] Vector addition.
- [ ] Scalar multiplication.
- [ ] Dot products.
- [ ] Matrix multiplication.
- [ ] Matrix transpose.
- [ ] Identity matrices.
- [ ] Matrix inverses.
- [ ] Systems of linear equations.
- [ ] Linear independence.
- [ ] Basis.
- [ ] Rank.
- [ ] Norms.
- [ ] Distance metrics.
- [ ] Cosine similarity.
- [ ] Eigenvalues.
- [ ] Eigenvectors.
- [ ] Singular Value Decomposition.
- [ ] Connect linear algebra concepts to embeddings and neural networks.

## 2.3 Calculus
- [ ] Functions and limits.
- [ ] Derivatives.
- [ ] Partial derivatives.
- [ ] Chain rule.
- [ ] Gradients.
- [ ] Directional derivatives.
- [ ] Multivariable functions.
- [ ] Gradient descent.
- [ ] Understand derivatives as rates of change.
- [ ] Understand gradients as directions of steepest increase.
- [ ] Understand why neural-network training requires derivatives.
- [ ] Derive simple gradients manually.

## 2.4 Probability
- [ ] Random variables.
- [ ] Probability distributions.
- [ ] Conditional probability.
- [ ] Independence.
- [ ] Bayes' theorem.
- [ ] Expected value.
- [ ] Variance.
- [ ] Standard deviation.
- [ ] Covariance.
- [ ] Bernoulli distribution.
- [ ] Binomial distribution.
- [ ] Normal distribution.
- [ ] Probability density functions.
- [ ] Cumulative distribution functions.
- [ ] Likelihood.
- [ ] Maximum likelihood estimation.

## 2.5 Statistics
- [ ] Population versus sample.
- [ ] Mean.
- [ ] Median.
- [ ] Mode.
- [ ] Variance.
- [ ] Standard deviation.
- [ ] Percentiles.
- [ ] Outliers.
- [ ] Correlation.
- [ ] Correlation versus causation.
- [ ] Sampling.
- [ ] Sampling bias.
- [ ] Confidence intervals.
- [ ] Hypothesis testing.
- [ ] Null and alternative hypotheses.
- [ ] p-values.
- [ ] Type I and Type II errors.
- [ ] Statistical significance versus practical significance.
- [ ] Basic experimental design.

## 2.6 Optimization
- [ ] Define an objective function.
- [ ] Define a loss function.
- [ ] Understand convex versus non-convex optimization.
- [ ] Gradient descent.
- [ ] Stochastic gradient descent.
- [ ] Mini-batch gradient descent.
- [ ] Learning rates.
- [ ] Local minima.
- [ ] Saddle points.
- [ ] Momentum.
- [ ] Understand why optimization is central to ML training.

### Phase 2 Implementation Exercises
- [ ] Implement vectors using NumPy.
- [ ] Implement matrix multiplication manually.
- [ ] Calculate cosine similarity manually.
- [ ] Calculate mean, variance, and standard deviation manually.
- [ ] Implement gradient descent for a simple mathematical function.
- [ ] Derive the gradient of mean squared error.
- [ ] Plot gradient descent converging toward a minimum.

### Phase 2 Exit Criteria
- [ ] Explain dot products geometrically.
- [ ] Explain matrix multiplication in the context of neural networks.
- [ ] Explain derivatives and gradients.
- [ ] Explain probability versus likelihood.
- [ ] Explain gradient descent mathematically and intuitively.

---

# Phase 3 — Data Science Foundations

## 3.1 The Data Science Lifecycle
- [ ] Define the problem.
- [ ] Define measurable success criteria.
- [ ] Acquire data.
- [ ] Understand data provenance.
- [ ] Inspect data quality.
- [ ] Clean data.
- [ ] Explore data.
- [ ] Engineer features.
- [ ] Build models.
- [ ] Evaluate models.
- [ ] Communicate results.
- [ ] Deploy models.
- [ ] Monitor models.
- [ ] Iterate.

## 3.2 Data Quality
- [ ] Missing data.
- [ ] Invalid values.
- [ ] Duplicate records.
- [ ] Outliers.
- [ ] Inconsistent formats.
- [ ] Data leakage.
- [ ] Sampling bias.
- [ ] Class imbalance.
- [ ] Label quality.
- [ ] Data drift.
- [ ] Concept drift.

## 3.3 SQL for AI and Data Science
- [ ] `SELECT`.
- [ ] `WHERE`.
- [ ] `ORDER BY`.
- [ ] `GROUP BY`.
- [ ] Aggregate functions.
- [ ] `JOIN`.
- [ ] Subqueries.
- [ ] Common Table Expressions.
- [ ] Window functions.
- [ ] Basic database normalization.
- [ ] Index fundamentals.
- [ ] Query-performance fundamentals.
- [ ] Connect Python to a relational database.
- [ ] Load SQL results into pandas.

## 3.4 Feature Engineering
- [ ] Numerical features.
- [ ] Categorical features.
- [ ] Ordinal features.
- [ ] Binary features.
- [ ] Date/time features.
- [ ] Encoding categorical variables.
- [ ] One-hot encoding.
- [ ] Normalization.
- [ ] Standardization.
- [ ] Log transformations.
- [ ] Binning.
- [ ] Handling missing values.
- [ ] Feature interactions.
- [ ] Avoid feature leakage.

### Phase 3 Project
- [ ] Define a business question.
- [ ] Acquire a dataset.
- [ ] Document its schema.
- [ ] Perform data-quality analysis.
- [ ] Perform exploratory analysis.
- [ ] Engineer candidate features.
- [ ] Write a concise findings report.

---

# Phase 4 — Classical Machine Learning

## 4.1 Core ML Concepts
- [ ] Understand supervised learning.
- [ ] Understand unsupervised learning.
- [ ] Understand regression.
- [ ] Understand classification.
- [ ] Understand clustering.
- [ ] Understand dimensionality reduction.
- [ ] Understand training data.
- [ ] Understand validation data.
- [ ] Understand test data.
- [ ] Understand generalization.
- [ ] Understand underfitting.
- [ ] Understand overfitting.
- [ ] Understand bias.
- [ ] Understand variance.
- [ ] Understand the bias-variance tradeoff.
- [ ] Understand regularization.
- [ ] Understand cross-validation.

## 4.2 Regression
- [ ] Simple linear regression.
- [ ] Multiple linear regression.
- [ ] Mean squared error.
- [ ] Mean absolute error.
- [ ] Root mean squared error.
- [ ] R².
- [ ] L1 regularization.
- [ ] L2 regularization.
- [ ] Ridge regression.
- [ ] Lasso regression.

## 4.3 Classification
- [ ] Logistic regression.
- [ ] Sigmoid function.
- [ ] Decision boundaries.
- [ ] Binary classification.
- [ ] Multiclass classification.
- [ ] Confusion matrix.
- [ ] Accuracy.
- [ ] Precision.
- [ ] Recall.
- [ ] F1 score.
- [ ] Specificity.
- [ ] ROC curves.
- [ ] ROC-AUC.
- [ ] Precision-recall curves.
- [ ] Probability calibration.
- [ ] Classification thresholds.

## 4.4 Instance-Based and Margin Models
- [ ] k-Nearest Neighbors.
- [ ] Distance metrics.
- [ ] Support Vector Machines.
- [ ] Maximum-margin intuition.
- [ ] Kernel intuition.

## 4.5 Decision Trees
- [ ] Tree structure.
- [ ] Splitting criteria.
- [ ] Gini impurity.
- [ ] Entropy.
- [ ] Information gain.
- [ ] Tree depth.
- [ ] Pruning.
- [ ] Overfitting in decision trees.

## 4.6 Ensemble Learning
- [ ] Bagging.
- [ ] Random forests.
- [ ] Boosting.
- [ ] Gradient boosting.
- [ ] XGBoost concepts.
- [ ] LightGBM concepts.
- [ ] Ensemble tradeoffs.

## 4.7 Unsupervised Learning
- [ ] k-Means clustering.
- [ ] Choosing `k`.
- [ ] Hierarchical clustering.
- [ ] DBSCAN concepts.
- [ ] Cluster evaluation.
- [ ] Principal Component Analysis.
- [ ] Dimensionality reduction.
- [ ] Visualization of high-dimensional data.
- [ ] Understand t-SNE conceptually.
- [ ] Understand UMAP conceptually.

## 4.8 Model Selection
- [ ] Baseline models.
- [ ] Train/validation/test splitting.
- [ ] k-fold cross-validation.
- [ ] Stratified splitting.
- [ ] Grid search.
- [ ] Random search.
- [ ] Hyperparameter optimization concepts.
- [ ] Learning curves.
- [ ] Validation curves.

## 4.9 scikit-learn
- [ ] Estimator API.
- [ ] `fit`.
- [ ] `predict`.
- [ ] `predict_proba`.
- [ ] Transformers.
- [ ] Pipelines.
- [ ] `ColumnTransformer`.
- [ ] Preprocessing pipelines.
- [ ] Model evaluation.
- [ ] Cross-validation.
- [ ] Hyperparameter search.
- [ ] Prevent preprocessing leakage.

## 4.10 Interpretability
- [ ] Feature importance.
- [ ] Permutation importance.
- [ ] Partial dependence concepts.
- [ ] SHAP concepts.
- [ ] Distinguish model explanation from causal explanation.

### Phase 4 From-Scratch Implementations
- [ ] Implement linear regression using NumPy.
- [ ] Implement gradient descent for linear regression.
- [ ] Implement logistic regression using NumPy.
- [ ] Implement k-Nearest Neighbors.
- [ ] Implement k-Means.
- [ ] Implement a basic decision tree or tree-splitting algorithm.
- [ ] Compare each implementation against scikit-learn.

### Phase 4 Project
- [ ] Select a supervised-learning problem.
- [ ] Establish a baseline.
- [ ] Build a preprocessing pipeline.
- [ ] Train at least three different model families.
- [ ] Evaluate with appropriate metrics.
- [ ] Perform cross-validation.
- [ ] Tune hyperparameters.
- [ ] Analyze errors.
- [ ] Explain the selected model.
- [ ] Produce a reproducible inference pipeline.

### Phase 4 Exit Criteria
- [ ] Determine whether a problem is regression, classification, clustering, or another ML problem.
- [ ] Select appropriate evaluation metrics.
- [ ] Detect obvious overfitting.
- [ ] Build a leakage-safe scikit-learn pipeline.
- [ ] Explain why one model performs better than another.

---

# Phase 5 — Neural Networks From Scratch

## 5.1 Neural Network Fundamentals
- [ ] Understand biological-neuron inspiration without confusing it with actual neuroscience.
- [ ] Artificial neurons.
- [ ] Inputs.
- [ ] Weights.
- [ ] Biases.
- [ ] Weighted sums.
- [ ] Activation functions.
- [ ] Layers.
- [ ] Input layers.
- [ ] Hidden layers.
- [ ] Output layers.
- [ ] Forward propagation.

## 5.2 Activation Functions
- [ ] Sigmoid.
- [ ] Tanh.
- [ ] ReLU.
- [ ] Leaky ReLU.
- [ ] GELU.
- [ ] Softmax.
- [ ] Understand why nonlinearity is necessary.

## 5.3 Loss Functions
- [ ] Mean squared error.
- [ ] Binary cross-entropy.
- [ ] Categorical cross-entropy.
- [ ] Negative log-likelihood.

## 5.4 Backpropagation
- [ ] Computational graphs.
- [ ] Chain rule.
- [ ] Local derivatives.
- [ ] Gradient propagation.
- [ ] Weight gradients.
- [ ] Bias gradients.
- [ ] Understand automatic differentiation.

## 5.5 Training
- [ ] Weight initialization.
- [ ] Forward pass.
- [ ] Loss calculation.
- [ ] Backward pass.
- [ ] Parameter update.
- [ ] Epochs.
- [ ] Batches.
- [ ] Mini-batches.
- [ ] Learning rates.
- [ ] Vanishing gradients.
- [ ] Exploding gradients.
- [ ] Gradient clipping.

### Phase 5 From-Scratch Project
- [ ] Build a neuron using only Python/NumPy.
- [ ] Build a dense layer using NumPy.
- [ ] Build an activation layer.
- [ ] Build a loss function.
- [ ] Implement backpropagation manually.
- [ ] Train a multilayer neural network without PyTorch or TensorFlow.
- [ ] Verify gradients numerically.
- [ ] Train the network on a small classification problem.
- [ ] Plot its learning curve.

### Phase 5 Exit Criteria
- [ ] Explain every calculation in a forward pass.
- [ ] Explain every major calculation in backpropagation.
- [ ] Explain why gradients update model weights.
- [ ] Train a small neural network without a deep-learning framework.

---

# Phase 6 — Deep Learning with PyTorch

## 6.1 PyTorch Fundamentals
- [ ] Tensors.
- [ ] Tensor shapes.
- [ ] Tensor data types.
- [ ] Tensor devices.
- [ ] CPU tensors.
- [ ] GPU tensors.
- [ ] Tensor operations.
- [ ] Broadcasting.
- [ ] Automatic differentiation.
- [ ] `requires_grad`.
- [ ] Computational graphs.
- [ ] `backward`.
- [ ] Gradients.
- [ ] `torch.nn.Module`.
- [ ] Layers.
- [ ] Loss functions.
- [ ] Optimizers.
- [ ] Datasets.
- [ ] DataLoaders.

## 6.2 Training Loops
- [ ] Build a training loop manually.
- [ ] Build a validation loop.
- [ ] Reset gradients correctly.
- [ ] Forward pass.
- [ ] Loss calculation.
- [ ] Backpropagation.
- [ ] Optimizer step.
- [ ] Track metrics.
- [ ] Save checkpoints.
- [ ] Load checkpoints.
- [ ] Reproduce experiments with seeds.

## 6.3 Optimization
- [ ] SGD.
- [ ] Momentum.
- [ ] Adam.
- [ ] AdamW.
- [ ] Weight decay.
- [ ] Learning-rate schedules.
- [ ] Early stopping.
- [ ] Dropout.
- [ ] Batch normalization.
- [ ] Layer normalization.

## 6.4 Convolutional Neural Networks
- [ ] Image tensors.
- [ ] Convolution.
- [ ] Filters/kernels.
- [ ] Stride.
- [ ] Padding.
- [ ] Pooling.
- [ ] Feature maps.
- [ ] CNN architectures.
- [ ] Transfer learning.
- [ ] Image augmentation.

## 6.5 Sequence Models
- [ ] Sequence data.
- [ ] Recurrent Neural Networks.
- [ ] Hidden state.
- [ ] Backpropagation through time.
- [ ] LSTM.
- [ ] GRU.
- [ ] Limitations of recurrent architectures.
- [ ] Understand why attention became important.

### Phase 6 Projects
- [ ] Build an MLP classifier in PyTorch.
- [ ] Build an image classifier with a CNN.
- [ ] Use transfer learning on an image dataset.
- [ ] Build a simple sequence model.
- [ ] Compare CPU and GPU training.
- [ ] Save and restore trained models.

### Phase 6 Exit Criteria
- [ ] Write a complete PyTorch training loop without copying a template.
- [ ] Diagnose common tensor-shape errors.
- [ ] Move a model between CPU and GPU.
- [ ] Save, load, and perform inference with a trained model.

---

# Phase 7 — Natural Language Processing

## 7.1 Text Fundamentals
- [ ] Text normalization.
- [ ] Sentence segmentation.
- [ ] Word tokenization.
- [ ] Stop words.
- [ ] Stemming.
- [ ] Lemmatization.
- [ ] n-grams.
- [ ] Bag of Words.
- [ ] TF-IDF.
- [ ] Sparse vectors.

## 7.2 Word Representations
- [ ] One-hot representations.
- [ ] Dense embeddings.
- [ ] Word2Vec.
- [ ] CBOW.
- [ ] Skip-gram.
- [ ] GloVe concepts.
- [ ] Semantic similarity.
- [ ] Cosine similarity.
- [ ] Embedding spaces.

## 7.3 NLP Tasks
- [ ] Text classification.
- [ ] Sentiment analysis.
- [ ] Named Entity Recognition.
- [ ] Information extraction.
- [ ] Question answering.
- [ ] Summarization.
- [ ] Translation.
- [ ] Semantic search.

### Phase 7 Project
- [ ] Build a TF-IDF text classifier.
- [ ] Build an embedding-based semantic search prototype.
- [ ] Compare lexical search against semantic search.

---

# Phase 8 — Attention and Transformers From Scratch

## 8.1 Attention
- [ ] Understand limitations of recurrence.
- [ ] Queries.
- [ ] Keys.
- [ ] Values.
- [ ] Dot-product attention.
- [ ] Scaled dot-product attention.
- [ ] Attention weights.
- [ ] Self-attention.
- [ ] Cross-attention.
- [ ] Causal masking.
- [ ] Padding masks.

## 8.2 Multi-Head Attention
- [ ] Understand attention heads.
- [ ] Projection matrices.
- [ ] Concatenating heads.
- [ ] Output projections.
- [ ] Understand why different heads can learn different relationships.

## 8.3 Transformer Architecture
- [ ] Token embeddings.
- [ ] Positional encoding.
- [ ] Positional embeddings.
- [ ] Residual connections.
- [ ] Layer normalization.
- [ ] Feed-forward networks.
- [ ] Transformer encoder.
- [ ] Transformer decoder.
- [ ] Encoder-decoder transformers.
- [ ] Decoder-only transformers.
- [ ] Encoder-only transformers.

## 8.4 Transformer Families
- [ ] Understand BERT-style encoder models.
- [ ] Understand GPT-style decoder models.
- [ ] Understand T5-style encoder-decoder models.
- [ ] Understand the architectural differences between these families.

### Phase 8 From-Scratch Project
- [ ] Implement scaled dot-product attention using NumPy or PyTorch primitives.
- [ ] Implement multi-head attention.
- [ ] Implement positional encoding.
- [ ] Implement a transformer block.
- [ ] Build a small character- or token-level transformer.
- [ ] Train it on a small corpus.
- [ ] Generate text autoregressively.

### Phase 8 Exit Criteria
- [ ] Explain attention mathematically.
- [ ] Explain queries, keys, and values intuitively.
- [ ] Explain causal masking.
- [ ] Trace a token through a transformer block.
- [ ] Explain the difference between encoder-only, decoder-only, and encoder-decoder transformers.

---

# Phase 9 — Large Language Models

## 9.1 Tokenization
- [ ] Characters versus words versus subwords.
- [ ] Vocabulary.
- [ ] Byte Pair Encoding.
- [ ] WordPiece concepts.
- [ ] SentencePiece concepts.
- [ ] Token IDs.
- [ ] Special tokens.
- [ ] Context windows.
- [ ] Understand why token counts differ from word counts.

## 9.2 Language Modeling
- [ ] Autoregressive prediction.
- [ ] Next-token prediction.
- [ ] Logits.
- [ ] Softmax probabilities.
- [ ] Cross-entropy loss.
- [ ] Perplexity.
- [ ] Sampling.

## 9.3 LLM Training Lifecycle
- [ ] Data collection.
- [ ] Data filtering.
- [ ] Deduplication.
- [ ] Tokenization.
- [ ] Pretraining.
- [ ] Continued pretraining.
- [ ] Supervised fine-tuning.
- [ ] Instruction tuning.
- [ ] Preference optimization.
- [ ] RLHF concepts.
- [ ] Reward models.
- [ ] PPO concepts.
- [ ] DPO concepts.
- [ ] Model evaluation.
- [ ] Deployment.
- [ ] Inference optimization.

## 9.4 Inference
- [ ] Temperature.
- [ ] Top-k.
- [ ] Top-p.
- [ ] Greedy decoding.
- [ ] Sampling.
- [ ] Stop sequences.
- [ ] Maximum output tokens.
- [ ] Context length.
- [ ] KV cache.
- [ ] Batch inference.
- [ ] Streaming.
- [ ] Quantization concepts.
- [ ] Model latency.
- [ ] Time to first token.
- [ ] Tokens per second.

## 9.5 LLM Limitations
- [ ] Hallucination.
- [ ] Stale knowledge.
- [ ] Prompt sensitivity.
- [ ] Context limitations.
- [ ] Lost-in-the-middle effects.
- [ ] Bias.
- [ ] Data contamination.
- [ ] Non-determinism.
- [ ] Prompt injection.
- [ ] Jailbreaking.
- [ ] Tool misuse.

### Phase 9 Project
- [ ] Use an open-weight transformer through Hugging Face.
- [ ] Inspect its tokenizer.
- [ ] Run inference.
- [ ] Compare decoding strategies.
- [ ] Inspect token probabilities.
- [ ] Evaluate outputs systematically.
- [ ] Fine-tune or parameter-efficiently adapt a small model.

---

# Phase 10 — Prompt Engineering and Structured LLM Applications

## 10.1 Prompt Design
- [ ] System instructions.
- [ ] User instructions.
- [ ] Context.
- [ ] Few-shot examples.
- [ ] Zero-shot prompting.
- [ ] Constraints.
- [ ] Output formatting.
- [ ] Delimiters.
- [ ] Prompt templates.
- [ ] Structured outputs.
- [ ] JSON schemas.
- [ ] Understand why prompt engineering cannot guarantee factual correctness.

## 10.2 LLM APIs
- [ ] Authentication.
- [ ] Request construction.
- [ ] Response parsing.
- [ ] Streaming.
- [ ] Retries.
- [ ] Exponential backoff.
- [ ] Rate limits.
- [ ] Timeouts.
- [ ] Token usage.
- [ ] Cost tracking.
- [ ] Error handling.
- [ ] Concurrency.

## 10.3 Evaluation
- [ ] Define evaluation datasets.
- [ ] Define evaluation criteria.
- [ ] Exact-match evaluation.
- [ ] Semantic similarity evaluation.
- [ ] Classification-based evaluation.
- [ ] Human evaluation.
- [ ] LLM-as-judge concepts.
- [ ] Understand biases in LLM-based evaluation.
- [ ] Regression testing for prompts.
- [ ] Track prompt/model versions.

### Phase 10 Project
- [ ] Build a structured LLM application.
- [ ] Require schema-valid output.
- [ ] Validate model responses.
- [ ] Retry malformed responses safely.
- [ ] Create an evaluation dataset.
- [ ] Compare multiple prompt versions quantitatively.

---

# Phase 11 — Embeddings, Vector Search, and RAG

## 11.1 Embeddings
- [ ] Understand embedding vectors.
- [ ] Embedding dimensionality.
- [ ] Semantic similarity.
- [ ] Cosine similarity.
- [ ] Dot-product similarity.
- [ ] Euclidean distance.
- [ ] Dense retrieval.
- [ ] Sparse retrieval.
- [ ] Hybrid retrieval.

## 11.2 Vector Search
- [ ] Vector indexes.
- [ ] Exact nearest-neighbor search.
- [ ] Approximate nearest-neighbor search.
- [ ] HNSW concepts.
- [ ] IVF concepts.
- [ ] Similarity thresholds.
- [ ] Metadata filtering.
- [ ] Understand retrieval recall versus latency.

## 11.3 RAG Architecture
- [ ] Document ingestion.
- [ ] Parsing.
- [ ] Cleaning.
- [ ] Chunking.
- [ ] Chunk overlap.
- [ ] Metadata generation.
- [ ] Embedding generation.
- [ ] Vector storage.
- [ ] Query embedding.
- [ ] Retrieval.
- [ ] Reranking.
- [ ] Context construction.
- [ ] Generation.
- [ ] Citations.
- [ ] Grounded-answer evaluation.

## 11.4 Advanced RAG
- [ ] Query rewriting.
- [ ] Multi-query retrieval.
- [ ] Hybrid search.
- [ ] Reranking models.
- [ ] Parent-child retrieval.
- [ ] Contextual chunking.
- [ ] Metadata-aware retrieval.
- [ ] Context compression.
- [ ] Retrieval evaluation.
- [ ] Faithfulness evaluation.
- [ ] Detect unanswerable questions.
- [ ] RAG security.
- [ ] Prompt-injection risks from retrieved documents.

### Phase 11 From-Scratch Project
- [ ] Build a document chunker.
- [ ] Generate embeddings.
- [ ] Store embeddings.
- [ ] Implement cosine-similarity retrieval manually.
- [ ] Retrieve relevant chunks.
- [ ] Construct an LLM prompt using retrieved context.
- [ ] Produce citations to source chunks.
- [ ] Evaluate retrieval separately from generation.

### Phase 11 Production Project
- [ ] Build a complete RAG application.
- [ ] Add hybrid retrieval.
- [ ] Add reranking.
- [ ] Add metadata filters.
- [ ] Add retrieval metrics.
- [ ] Add grounding evaluation.
- [ ] Add prompt-injection defenses.

---

# Phase 12 — Agentic AI

## 12.1 Agent Fundamentals
- [ ] Define an AI agent.
- [ ] Distinguish an agent from a chatbot.
- [ ] Distinguish an agent from a deterministic workflow.
- [ ] Understand the model → tool → observation → model loop.
- [ ] Understand state.
- [ ] Understand memory.
- [ ] Understand tools.
- [ ] Understand environment.
- [ ] Understand goals.
- [ ] Understand termination conditions.

## 12.2 Tool Use
- [ ] Function calling.
- [ ] Tool schemas.
- [ ] Argument validation.
- [ ] Tool selection.
- [ ] Tool execution.
- [ ] Tool-result handling.
- [ ] Error recovery.
- [ ] Idempotency.
- [ ] Side-effect management.
- [ ] Read tools versus write tools.
- [ ] Permission boundaries.

## 12.3 Agent Patterns
- [ ] ReAct concepts.
- [ ] Router pattern.
- [ ] Planner/executor pattern.
- [ ] Reflection concepts.
- [ ] Evaluator/optimizer pattern.
- [ ] Orchestrator/worker pattern.
- [ ] Human-in-the-loop workflows.
- [ ] Multi-agent systems.
- [ ] Understand when multi-agent architectures are unnecessary.

## 12.4 Memory
- [ ] Conversation history.
- [ ] Working memory.
- [ ] Long-term memory.
- [ ] Semantic memory.
- [ ] Episodic-memory concepts.
- [ ] Memory retrieval.
- [ ] Memory summarization.
- [ ] Memory expiration.
- [ ] Privacy implications of persistent memory.

## 12.5 Model Context Protocol
- [ ] Understand MCP's purpose.
- [ ] MCP clients.
- [ ] MCP servers.
- [ ] Tools.
- [ ] Resources.
- [ ] Prompts.
- [ ] Authentication and authorization.
- [ ] Security boundaries.
- [ ] Connect an agent to an MCP server.

## 12.6 Agent Reliability and Safety
- [ ] Maximum-step limits.
- [ ] Timeouts.
- [ ] Tool permissions.
- [ ] Input validation.
- [ ] Output validation.
- [ ] Human approval gates.
- [ ] Sandboxing.
- [ ] Audit logs.
- [ ] Prompt-injection defenses.
- [ ] Data-exfiltration risks.
- [ ] Tool-result poisoning.
- [ ] Infinite loops.
- [ ] Cascading failures.
- [ ] Cost limits.

## 12.7 Agent Evaluation
- [ ] Task-success rate.
- [ ] Tool-selection accuracy.
- [ ] Tool-argument accuracy.
- [ ] Number of steps.
- [ ] Latency.
- [ ] Cost.
- [ ] Safety violations.
- [ ] Human-intervention rate.
- [ ] Regression evaluation.

### Phase 12 From-Scratch Project
- [ ] Build a minimal agent loop without an agent framework.
- [ ] Define tool schemas manually.
- [ ] Execute tools.
- [ ] Return observations to the model.
- [ ] Add conversation state.
- [ ] Add maximum-step termination.
- [ ] Add error handling.
- [ ] Add approval before destructive actions.
- [ ] Add an evaluation suite.

### Phase 12 Framework Project
- [ ] Build the same agent using an established agent framework or SDK.
- [ ] Compare framework behavior with the from-scratch implementation.
- [ ] Identify what the framework abstracts.
- [ ] Identify where framework abstractions reduce control.

### Phase 12 Exit Criteria
- [ ] Explain an agent without referring to a specific framework.
- [ ] Build a tool-using agent from scratch.
- [ ] Explain when an ordinary workflow is preferable to an agent.
- [ ] Implement security boundaries around agent tools.

---

# Phase 13 — AI Application Engineering

## 13.1 Backend Development
- [ ] Build APIs using FastAPI.
- [ ] Request validation.
- [ ] Response models.
- [ ] Dependency injection concepts.
- [ ] Asynchronous endpoints.
- [ ] Authentication.
- [ ] Authorization.
- [ ] API versioning.
- [ ] Error responses.
- [ ] API documentation.

## 13.2 Application Architecture
- [ ] Separate presentation, application, domain, and infrastructure concerns.
- [ ] Separate model calls from business logic.
- [ ] Encapsulate external providers.
- [ ] Define clear data contracts.
- [ ] Handle retries centrally.
- [ ] Handle rate limiting.
- [ ] Handle timeouts.
- [ ] Implement caching.
- [ ] Implement queues where asynchronous work is appropriate.
- [ ] Implement bounded batch processing for large workloads.

## 13.3 Software Quality
- [ ] Unit testing.
- [ ] Integration testing.
- [ ] End-to-end testing.
- [ ] Mock external model APIs.
- [ ] Test model-independent business logic deterministically.
- [ ] Build evaluation tests for probabilistic model behavior.
- [ ] Static typing.
- [ ] Linting.
- [ ] Formatting.
- [ ] Dependency management.

## 13.4 Containers
- [ ] Understand containers.
- [ ] Install Docker.
- [ ] Create a Dockerfile.
- [ ] Build an image.
- [ ] Run a container.
- [ ] Environment variables.
- [ ] Volumes.
- [ ] Networking.
- [ ] Multi-stage builds.
- [ ] Container-security basics.

### Phase 13 Project
- [ ] Turn a previous ML or LLM prototype into a production-style API.
- [ ] Containerize it.
- [ ] Add tests.
- [ ] Add logging.
- [ ] Add configuration management.
- [ ] Add health checks.

---

# Phase 14 — MLOps and LLMOps

## 14.1 Reproducibility
- [ ] Version code.
- [ ] Version datasets.
- [ ] Version models.
- [ ] Version prompts.
- [ ] Version configuration.
- [ ] Track experiments.
- [ ] Record random seeds.
- [ ] Record dependencies.

## 14.2 ML Lifecycle
- [ ] Training pipelines.
- [ ] Validation pipelines.
- [ ] Model registry.
- [ ] Model promotion.
- [ ] Deployment.
- [ ] Rollback.
- [ ] Scheduled retraining.
- [ ] Trigger-based retraining.
- [ ] Batch inference.
- [ ] Online inference.

## 14.3 Monitoring
- [ ] Infrastructure metrics.
- [ ] Latency.
- [ ] Throughput.
- [ ] Error rates.
- [ ] Data drift.
- [ ] Prediction drift.
- [ ] Concept drift.
- [ ] Model quality.
- [ ] Token usage.
- [ ] LLM cost.
- [ ] Retrieval quality.
- [ ] Hallucination/grounding metrics.
- [ ] Agent task-success metrics.

## 14.4 CI/CD
- [ ] Automated tests.
- [ ] Build pipelines.
- [ ] Deployment pipelines.
- [ ] Environment promotion.
- [ ] Secrets management.
- [ ] Infrastructure as Code concepts.
- [ ] Automated rollback strategies.

### Phase 14 Project
- [ ] Create an end-to-end ML pipeline.
- [ ] Train a model.
- [ ] Evaluate it automatically.
- [ ] Register the model.
- [ ] Deploy it.
- [ ] Monitor it.
- [ ] Trigger or simulate retraining.
- [ ] Maintain reproducibility across runs.

---

# Phase 15 — AI Security, Governance, and Responsible AI

## 15.1 Security Foundations
- [ ] Least privilege.
- [ ] Secrets management.
- [ ] Encryption at rest.
- [ ] Encryption in transit.
- [ ] Network isolation.
- [ ] Authentication.
- [ ] Authorization.
- [ ] Audit logging.
- [ ] Dependency security.
- [ ] Data classification.

## 15.2 AI-Specific Security
- [ ] Prompt injection.
- [ ] Indirect prompt injection.
- [ ] Jailbreaking.
- [ ] Data exfiltration.
- [ ] Model extraction concepts.
- [ ] Training-data poisoning.
- [ ] RAG poisoning.
- [ ] Tool abuse.
- [ ] Excessive agency.
- [ ] Insecure output handling.
- [ ] Sensitive-information disclosure.

## 15.3 Responsible AI
- [ ] Bias.
- [ ] Fairness.
- [ ] Explainability.
- [ ] Transparency.
- [ ] Privacy.
- [ ] Human oversight.
- [ ] Model limitations.
- [ ] Dataset documentation.
- [ ] Evaluation across user populations.
- [ ] Risk-based deployment decisions.

---

# Phase 16 — Cloud Fundamentals for OCI

## 16.1 OCI Core Concepts
- [ ] Tenancies.
- [ ] Regions.
- [ ] Availability Domains.
- [ ] Fault Domains.
- [ ] Compartments.
- [ ] OCIDs.
- [ ] Resource limits.
- [ ] Tags.

## 16.2 OCI IAM
- [ ] Users.
- [ ] Groups.
- [ ] Dynamic groups.
- [ ] Domains.
- [ ] Policies.
- [ ] Policy verbs.
  - [ ] inspect
  - [ ] read
  - [ ] use
  - [ ] manage
- [ ] Resource principals.
- [ ] Instance principals.
- [ ] Least-privilege policy design.

## 16.3 OCI Networking
- [ ] Virtual Cloud Networks.
- [ ] CIDR ranges.
- [ ] Subnets.
- [ ] Public versus private subnets.
- [ ] Route tables.
- [ ] Security lists.
- [ ] Network Security Groups.
- [ ] Internet Gateway.
- [ ] NAT Gateway.
- [ ] Service Gateway.
- [ ] DNS.
- [ ] Private endpoints.
- [ ] Load balancers.

## 16.4 OCI Storage and Data
- [ ] Object Storage.
- [ ] Buckets.
- [ ] Objects.
- [ ] Block Volume concepts.
- [ ] File Storage concepts.
- [ ] Autonomous AI Database fundamentals.
- [ ] Database connection fundamentals.

## 16.5 OCI Application Services
- [ ] OCI Functions.
- [ ] API Gateway.
- [ ] Container Registry.
- [ ] Container Instances concepts.
- [ ] Oracle Kubernetes Engine concepts.
- [ ] Events.
- [ ] Notifications.
- [ ] Streaming concepts.

## 16.6 OCI Operations
- [ ] Logging.
- [ ] Monitoring.
- [ ] Metrics.
- [ ] Alarms.
- [ ] Notifications.
- [ ] Vault.
- [ ] Secrets.
- [ ] Cloud Shell.
- [ ] OCI CLI.
- [ ] OCI Python SDK.
- [ ] Resource Manager / Terraform concepts.

### Phase 16 Project
- [ ] Create an OCI development compartment.
- [ ] Configure IAM.
- [ ] Create an Object Storage bucket.
- [ ] Access OCI from Python using the OCI SDK.
- [ ] Upload and download data programmatically.
- [ ] Configure secure authentication.
- [ ] Enable logging and monitoring.

---

# Phase 17 — OCI Data Science

- [ ] Understand OCI Data Science architecture.
- [ ] Create a Data Science project.
- [ ] Create a notebook session.
- [ ] Use JupyterLab in OCI Data Science.
- [ ] Configure Conda environments.
- [ ] Understand Oracle Accelerated Data Science SDK.
- [ ] Use ADS to access data.
- [ ] Profile datasets.
- [ ] Prepare datasets.
- [ ] Train models.
- [ ] Evaluate models.
- [ ] Explain models.
- [ ] Explore Oracle AutoML.
- [ ] Understand the model catalog.
- [ ] Save models to the model catalog.
- [ ] Understand model artifacts.
- [ ] Create model deployments.
- [ ] Invoke deployed models through HTTP endpoints.
- [ ] Configure model-deployment networking.
- [ ] Configure model-deployment authentication.
- [ ] Create Data Science jobs.
- [ ] Run repeatable training jobs.
- [ ] Run batch inference jobs.
- [ ] Create Data Science pipelines.
- [ ] Build an end-to-end ML pipeline.
- [ ] Configure logs.
- [ ] Configure metrics.
- [ ] Configure alarms.
- [ ] Use GPUs where appropriate.
- [ ] Understand distributed training concepts.
- [ ] Explore Data Science AI Operators.
- [ ] Explore AI Quick Actions.
- [ ] Use AI Quick Actions for supported foundation-model workflows.
- [ ] Understand OCI Data Science MLOps patterns.

### Phase 17 OCI Project
- [ ] Rebuild the Phase 4 ML project inside OCI Data Science.
- [ ] Store source data in Object Storage.
- [ ] Train the model in an OCI notebook.
- [ ] Register the model.
- [ ] Deploy the model as an HTTP endpoint.
- [ ] Call the endpoint from a separate application.
- [ ] Create a repeatable training job.
- [ ] Build a Data Science pipeline.
- [ ] Add logging and monitoring.

### Phase 17 Reference Verification
- [ ] Review the current OCI Data Science documentation before implementation because OCI capabilities change over time. OCI currently describes Data Science as its managed platform for notebooks, model training, model catalog, model deployments, jobs, pipelines, ADS, AutoML, and related ML lifecycle capabilities. ([docs.oracle.com](https://docs.oracle.com/iaas/data-science/using/overview.htm))

---

# Phase 18 — OCI Prebuilt AI Services

## 18.1 OCI Language
- [ ] Understand OCI Language.
- [ ] Language detection.
- [ ] Text classification.
- [ ] Named Entity Recognition.
- [ ] Key-phrase extraction.
- [ ] Sentiment analysis.
- [ ] Text translation.
- [ ] PII detection and de-identification.
- [ ] Custom text-classification models.
- [ ] Custom NER models.
- [ ] Call Language through the OCI SDK.
- [ ] Compare a prebuilt Language service against a custom ML/LLM implementation.
- [ ] Review current OCI Language capabilities before implementation. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/language/using/overview.htm))

## 18.2 OCI Speech
- [ ] Understand speech recognition.
- [ ] Create transcription jobs.
- [ ] Process audio stored in Object Storage.
- [ ] Parse timestamped transcription output.
- [ ] Explore Live Transcribe.
- [ ] Explore transcription customization.
- [ ] Explore supported multilingual models.
- [ ] Explore Whisper-based transcription where supported.
- [ ] Explore OCI Text to Speech where available.
- [ ] Build a speech-to-text application.
- [ ] Review current OCI Speech capabilities and regional availability before implementation. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/speech/using/speech.htm))

## 18.3 OCI Vision
- [ ] Understand image classification.
- [ ] Understand object detection.
- [ ] Use pretrained Vision models.
- [ ] Analyze images through the API.
- [ ] Perform asynchronous batch image processing.
- [ ] Train a supported custom Vision model.
- [ ] Explore stored-video analysis where applicable.
- [ ] Explore stream-video analysis where applicable.
- [ ] Review current OCI Vision capabilities and regional availability before implementation. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/vision/using/overview.htm))

## 18.4 OCI Document Understanding
- [ ] Understand OCR.
- [ ] Extract document text.
- [ ] Extract key-value pairs.
- [ ] Extract tables.
- [ ] Classify documents.
- [ ] Generate searchable OCR PDFs.
- [ ] Process documents individually.
- [ ] Process documents in batches.
- [ ] Explore custom classic models.
- [ ] Explore current generative extraction capabilities.
- [ ] Build an automated document-processing pipeline.
- [ ] Review current OCI Document Understanding capabilities before implementation. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/document-understanding/using/overview.htm))

## 18.5 OCI Data Labeling
- [ ] Understand when labeled datasets are required.
- [ ] Create labeling datasets.
- [ ] Define labeling classes.
- [ ] Perform image labeling.
- [ ] Perform text labeling where supported.
- [ ] Export labeled datasets.
- [ ] Connect labeled data to model-training workflows.
- [ ] Understand labeling-quality assurance.

### Phase 18 Integration Project
- [ ] Build one application combining at least two OCI AI Services.
- [ ] Store inputs and outputs in Object Storage.
- [ ] Access services through the OCI SDK.
- [ ] Apply IAM least privilege.
- [ ] Add monitoring.
- [ ] Compare managed AI Services against custom-model approaches.

---

# Phase 19 — OCI Generative AI

## 19.1 OCI Generative AI Foundations
- [ ] Understand OCI Generative AI architecture.
- [ ] Understand available model families.
- [ ] Understand model availability by region.
- [ ] Use the OCI Generative AI playground.
- [ ] Call models through the OCI SDK/API.
- [ ] Understand OCI's OpenAI-compatible APIs.
- [ ] Use chat models.
- [ ] Use embedding models.
- [ ] Use reranking models.
- [ ] Understand model parameters.
- [ ] Stream responses.
- [ ] Track token usage.
- [ ] Handle service limits.
- [ ] Configure IAM permissions.
- [ ] Configure private networking where required.
- [ ] Review current OCI Generative AI models and regional availability before every implementation. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/generative-ai/home.htm))

## 19.2 OCI Embeddings and Reranking
- [ ] Generate embeddings.
- [ ] Store embedding vectors.
- [ ] Perform semantic retrieval.
- [ ] Use reranking.
- [ ] Measure retrieval improvements produced by reranking.
- [ ] Build a semantic-search application.

## 19.3 Customization and Model Hosting
- [ ] Understand pretrained versus custom models.
- [ ] Understand model fine-tuning.
- [ ] Understand model importing.
- [ ] Understand dedicated AI clusters.
- [ ] Understand hosting dedicated AI clusters.
- [ ] Understand fine-tuning dedicated AI clusters.
- [ ] Understand capacity and service-limit requirements.
- [ ] Understand when on-demand inference is preferable.
- [ ] Understand when dedicated hosting is justified.
- [ ] Fine-tune a supported model when practical.
- [ ] Deploy a custom or imported model when practical.
- [ ] Review current dedicated-cluster requirements before implementation. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/generative-ai/limits.htm))

## 19.4 OCI Generative AI Governance
- [ ] Study OCI Generative AI IAM.
- [ ] Study guardrails.
- [ ] Study content-safety controls.
- [ ] Study private endpoints.
- [ ] Study auditability.
- [ ] Study observability.
- [ ] Apply least privilege to generative-AI applications.
- [ ] Separate development and production resources.
- [ ] Establish model and prompt evaluation gates.

### Phase 19 Project
- [ ] Build an OCI-hosted generative-AI application.
- [ ] Call OCI Generative AI from Python.
- [ ] Implement streaming.
- [ ] Implement structured output.
- [ ] Add retries and rate-limit handling.
- [ ] Add an evaluation suite.
- [ ] Add logging.
- [ ] Add guardrails.
- [ ] Add cost/usage tracking.

---

# Phase 20 — Oracle Database AI Vector Search and OCI RAG

## 20.1 Database Foundations for RAG
- [ ] Review Oracle Database architecture relevant to application development.
- [ ] Understand Autonomous AI Database.
- [ ] Understand database authentication.
- [ ] Understand connection pooling.
- [ ] Understand database security and IAM integration.

## 20.2 AI Vector Search
- [ ] Study Oracle Database vector data types.
- [ ] Store embeddings in Oracle Database.
- [ ] Perform vector similarity search.
- [ ] Create vector indexes.
- [ ] Compare exact and approximate search.
- [ ] Combine relational filters with vector search.
- [ ] Build hybrid structured + semantic queries.
- [ ] Measure recall and latency.

## 20.3 OCI RAG Project
- [ ] Ingest documents.
- [ ] Parse documents.
- [ ] Chunk documents.
- [ ] Generate embeddings using OCI Generative AI.
- [ ] Store vectors using the selected OCI-supported vector architecture.
- [ ] Perform semantic search.
- [ ] Rerank retrieved documents.
- [ ] Generate grounded answers.
- [ ] Return source citations.
- [ ] Evaluate retrieval.
- [ ] Evaluate answer faithfulness.
- [ ] Add authorization filters so users cannot retrieve documents they cannot access.

---

# Phase 21 — OCI Enterprise AI Agents

## 21.1 OCI Agent Architecture
- [ ] Understand OCI's current Enterprise AI Agents architecture.
- [ ] Understand the OCI Responses API.
- [ ] Understand hosted agentic applications.
- [ ] Understand when to use an API-first agent.
- [ ] Understand when to use a hosted agentic application.
- [ ] Understand hybrid architectures.
- [ ] Review current architecture before implementation because OCI's agent platform is actively evolving. OCI currently identifies the Responses API and hosted agentic applications as its two primary approaches. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/generative-ai/agents.htm))

## 21.2 OCI Responses API
- [ ] Send model requests.
- [ ] Manage conversation state.
- [ ] Use supported reasoning capabilities where applicable.
- [ ] Use tool calling.
- [ ] Handle multi-step tool execution.
- [ ] Handle errors and termination.

## 21.3 OCI Agent Tools
- [ ] File Search.
- [ ] Vector Stores.
- [ ] Code Interpreter.
- [ ] Function Calling.
- [ ] MCP calling.
- [ ] SQL/NL2SQL capabilities.
- [ ] Understand which tools are OpenAI-compatible versus OCI-native.
- [ ] Review current tool support before implementation. OCI currently documents File Search, Code Interpreter, Function Calling, MCP calling, and OCI-native NL2SQL among its agent tooling. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/generative-ai/tool-support.htm))

## 21.4 Agent Memory
- [ ] Understand OCI agent conversation state.
- [ ] Understand supported memory mechanisms.
- [ ] Define what information should persist.
- [ ] Define memory-retention policies.
- [ ] Protect sensitive information.

## 21.5 Function Calling
- [ ] Define an OCI agent function tool.
- [ ] Create typed input schemas.
- [ ] Implement backend functions.
- [ ] Validate arguments.
- [ ] Add authorization.
- [ ] Add approval gates to sensitive operations.
- [ ] Handle failures safely.

## 21.6 RAG Agents
- [ ] Connect an agent to enterprise documents.
- [ ] Configure vector stores.
- [ ] Configure File Search/RAG tooling.
- [ ] Test retrieval.
- [ ] Add citations.
- [ ] Evaluate grounding.
- [ ] Apply document-level authorization.

## 21.7 SQL and NL2SQL Agents
- [ ] Understand natural-language-to-SQL architecture.
- [ ] Understand semantic enrichment.
- [ ] Understand schema mapping.
- [ ] Understand SQL-generation validation.
- [ ] Understand separation between SQL generation and SQL execution.
- [ ] Configure authorized database access.
- [ ] Restrict query permissions.
- [ ] Add human approval where appropriate.
- [ ] Build natural-language queries over enterprise data.
- [ ] Review OCI's current NL2SQL architecture before implementation. OCI currently documents Enterprise AI NL2SQL for generating validated SQL and separates generated SQL from authorized query execution. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/generative-ai/agents.htm))

## 21.8 OCI Agent Development Kit
- [ ] Study the OCI Agent Development Kit.
- [ ] Complete its Python quickstart.
- [ ] Build an agent using the ADK.
- [ ] Implement custom tools.
- [ ] Implement agent state.
- [ ] Add observability.
- [ ] Add evaluations.
- [ ] Compare the ADK implementation against the from-scratch Phase 12 agent.

### Phase 21 Project
- [ ] Build an enterprise agent using OCI.
- [ ] Add document retrieval.
- [ ] Add at least one custom function.
- [ ] Add structured-data access.
- [ ] Add agent memory/state where justified.
- [ ] Add authorization.
- [ ] Add human approval for sensitive write actions.
- [ ] Add observability.
- [ ] Add evaluation.
- [ ] Test prompt-injection attacks.
- [ ] Test unauthorized-data-access attempts.
- [ ] Measure task success, latency, and cost.

---

# Phase 22 — Advanced Model Training

## 22.1 Training at Scale
- [ ] GPU architecture basics.
- [ ] GPU memory.
- [ ] CPU ↔ GPU data transfer.
- [ ] Mixed-precision training.
- [ ] FP32.
- [ ] FP16.
- [ ] BF16.
- [ ] Gradient accumulation.
- [ ] Distributed training concepts.
- [ ] Data parallelism.
- [ ] Model parallelism.
- [ ] Tensor parallelism.
- [ ] Pipeline parallelism.
- [ ] Checkpointing.
- [ ] Gradient checkpointing.

## 22.2 Efficient Fine-Tuning
- [ ] Full fine-tuning.
- [ ] Parameter-efficient fine-tuning.
- [ ] LoRA.
- [ ] QLoRA.
- [ ] Adapter concepts.
- [ ] Dataset preparation.
- [ ] Instruction dataset formatting.
- [ ] Validation.
- [ ] Fine-tuning evaluation.
- [ ] Catastrophic forgetting.
- [ ] Overfitting during fine-tuning.

## 22.3 Model Compression and Inference
- [ ] Quantization.
- [ ] Distillation concepts.
- [ ] Pruning concepts.
- [ ] KV caching.
- [ ] Continuous batching concepts.
- [ ] Speculative decoding concepts.
- [ ] Inference-server architecture.
- [ ] Throughput versus latency tradeoffs.

### Phase 22 Project
- [ ] Fine-tune a small open-weight LLM.
- [ ] Compare base versus fine-tuned performance.
- [ ] Quantize the model.
- [ ] Benchmark inference.
- [ ] Document quality, memory, latency, and cost tradeoffs.

---

# Phase 23 — Advanced AI Architecture

## 23.1 Production RAG Architecture
- [ ] Data ingestion pipelines.
- [ ] Incremental indexing.
- [ ] Re-indexing.
- [ ] Embedding-version migrations.
- [ ] Document deletion.
- [ ] Access-control-aware retrieval.
- [ ] Multi-tenant vector search.
- [ ] Retrieval caching.
- [ ] Generation caching.
- [ ] Evaluation pipelines.

## 23.2 Production Agent Architecture
- [ ] Durable execution.
- [ ] State machines.
- [ ] Event-driven agents.
- [ ] Long-running workflows.
- [ ] Queue-backed tool execution.
- [ ] Idempotent actions.
- [ ] Retry policies.
- [ ] Dead-letter handling.
- [ ] Human approval workflows.
- [ ] Audit trails.
- [ ] Budget enforcement.

## 23.3 Scaling AI Systems
- [ ] Horizontal scaling.
- [ ] Vertical scaling.
- [ ] Load balancing.
- [ ] Autoscaling.
- [ ] Queue-based load leveling.
- [ ] Rate limiting.
- [ ] Backpressure.
- [ ] Caching.
- [ ] Batch processing.
- [ ] Request batching.
- [ ] GPU utilization.
- [ ] Capacity planning.

## 23.4 Reliability
- [ ] SLIs.
- [ ] SLOs.
- [ ] Error budgets.
- [ ] Circuit breakers.
- [ ] Graceful degradation.
- [ ] Provider/model fallback.
- [ ] Disaster recovery.
- [ ] Multi-region concepts.

---

# Phase 24 — End-to-End OCI AI Architecture

## 24.1 Architecture Design
- [ ] Define a real business problem.
- [ ] Define users.
- [ ] Define functional requirements.
- [ ] Define non-functional requirements.
- [ ] Define security requirements.
- [ ] Define availability requirements.
- [ ] Define latency requirements.
- [ ] Define expected workload.
- [ ] Define data sources.
- [ ] Define data-retention requirements.
- [ ] Define AI evaluation criteria.

## 24.2 OCI Architecture
- [ ] Design compartments.
- [ ] Design IAM policies.
- [ ] Design networking.
- [ ] Design private/public boundaries.
- [ ] Design storage.
- [ ] Design database architecture.
- [ ] Select appropriate OCI AI services.
- [ ] Select appropriate generative-AI models.
- [ ] Select model-serving architecture.
- [ ] Design RAG if required.
- [ ] Design agent architecture if required.
- [ ] Design application APIs.
- [ ] Design asynchronous processing.
- [ ] Design monitoring.
- [ ] Design logging.
- [ ] Design secrets management.
- [ ] Design CI/CD.
- [ ] Design disaster recovery.
- [ ] Estimate cost.

## 24.3 Implementation
- [ ] Provision infrastructure.
- [ ] Implement ingestion.
- [ ] Implement preprocessing.
- [ ] Implement AI/model layer.
- [ ] Implement retrieval.
- [ ] Implement tools.
- [ ] Implement agent orchestration where justified.
- [ ] Implement application backend.
- [ ] Implement authentication.
- [ ] Implement authorization.
- [ ] Implement observability.
- [ ] Implement evaluations.
- [ ] Implement automated tests.
- [ ] Implement deployment pipeline.

## 24.4 Validation
- [ ] Functional testing.
- [ ] Load testing.
- [ ] Security testing.
- [ ] Prompt-injection testing.
- [ ] Data-access testing.
- [ ] Model-quality evaluation.
- [ ] Retrieval evaluation.
- [ ] Agent evaluation.
- [ ] Cost evaluation.
- [ ] Failure-mode testing.

---

# Phase 25 — Final Capstone: Production OCI AI System

- [ ] Select a sufficiently complex real-world problem.
- [ ] Write requirements.
- [ ] Write a solution-design document.
- [ ] Create an architecture diagram.
- [ ] Create a data model.
- [ ] Create an evaluation plan.
- [ ] Create a security model.
- [ ] Create an OCI infrastructure design.
- [ ] Create the Python application.
- [ ] Create automated tests.
- [ ] Create an ML component where appropriate.
- [ ] Create an LLM component.
- [ ] Create a RAG component.
- [ ] Create an agentic component only where agent autonomy is justified.
- [ ] Integrate OCI Generative AI.
- [ ] Integrate OCI Data Science.
- [ ] Integrate at least one OCI prebuilt AI Service.
- [ ] Integrate Oracle Database/vector search where appropriate.
- [ ] Use Object Storage.
- [ ] Configure IAM with least privilege.
- [ ] Configure secure networking.
- [ ] Configure Vault/secrets.
- [ ] Configure Logging.
- [ ] Configure Monitoring.
- [ ] Configure alarms.
- [ ] Containerize application components where appropriate.
- [ ] Automate deployment.
- [ ] Implement model/LLM evaluation.
- [ ] Implement RAG evaluation.
- [ ] Implement agent evaluation.
- [ ] Implement application observability.
- [ ] Perform load testing.
- [ ] Perform security testing.
- [ ] Perform cost analysis.
- [ ] Document operational procedures.
- [ ] Document known limitations.
- [ ] Produce a complete architecture review.
- [ ] Deploy the final system to OCI.

---

# Phase 26 — OCI AI Coverage Audit

- [ ] Re-open the current OCI service catalog before declaring the roadmap complete.
- [ ] Compare this checklist against Oracle's current Analytics and AI service catalog.
- [ ] Identify AI services introduced after this roadmap was written.
- [ ] Identify deprecated or renamed services.
- [ ] Add newly relevant OCI AI capabilities to this checklist.
- [ ] Remove or archive obsolete learning objectives rather than learning deprecated implementations.
- [ ] Verify current OCI Data Science capabilities.
- [ ] Verify current OCI Generative AI capabilities.
- [ ] Verify current Enterprise AI Agents capabilities.
- [ ] Verify current Language capabilities.
- [ ] Verify current Speech capabilities.
- [ ] Verify current Vision capabilities.
- [ ] Verify current Document Understanding capabilities.
- [ ] Verify current Data Labeling capabilities.
- [ ] Verify current Oracle Database AI/vector capabilities.
- [ ] Verify current AI Data Platform capabilities.
- [ ] Review related OCI services that have become materially relevant to AI workloads.
- [ ] Update this master checklist before beginning any newly introduced service.
- [ ] Treat Oracle's current documentation as authoritative for OCI implementation details. Oracle's August 2026 service catalog currently lists Data Science, Data Labeling, Document Understanding, Generative AI, Generative AI Agents, Language, Speech, Vision, and AI Data Platform among its Analytics and AI services. ([docs.oracle.com](https://docs.oracle.com/en-us/iaas/Content/))

---

# Final Competency Checklist

## AI and Mathematics
- [ ] Explain the major branches of AI.
- [ ] Explain the mathematics behind classical ML.
- [ ] Explain gradient descent.
- [ ] Explain neural networks.
- [ ] Explain backpropagation.
- [ ] Explain attention.
- [ ] Explain transformers.
- [ ] Explain LLM training and inference.

## Data Science
- [ ] Explore unfamiliar datasets independently.
- [ ] Clean data appropriately.
- [ ] Detect common data-quality problems.
- [ ] Engineer useful features.
- [ ] Select appropriate metrics.
- [ ] Design valid experiments.

## Machine Learning
- [ ] Implement fundamental ML algorithms from scratch.
- [ ] Train standard models using scikit-learn.
- [ ] Detect overfitting and leakage.
- [ ] Tune and evaluate models correctly.
- [ ] Explain model predictions appropriately.

## Deep Learning
- [ ] Build neural networks from scratch.
- [ ] Train models using PyTorch.
- [ ] Use GPUs.
- [ ] Build CNNs.
- [ ] Build sequence models.
- [ ] Build transformer components.

## LLM Engineering
- [ ] Understand tokenization.
- [ ] Understand LLM inference.
- [ ] Use model APIs.
- [ ] Use structured outputs.
- [ ] Evaluate prompts and model outputs.
- [ ] Fine-tune a small model.
- [ ] Understand model-serving tradeoffs.

## RAG
- [ ] Generate embeddings.
- [ ] Perform vector retrieval.
- [ ] Build hybrid search.
- [ ] Implement reranking.
- [ ] Build production-style RAG.
- [ ] Evaluate retrieval independently from generation.
- [ ] Evaluate grounding and faithfulness.

## Agentic AI
- [ ] Build an agent without a framework.
- [ ] Use function/tool calling.
- [ ] Implement state and memory.
- [ ] Connect tools through MCP.
- [ ] Build agent workflows.
- [ ] Evaluate agent behavior.
- [ ] Secure agents against tool abuse and prompt injection.
- [ ] Decide when not to use an agent.

## Production Engineering
- [ ] Build AI APIs.
- [ ] Containerize AI applications.
- [ ] Test AI applications.
- [ ] Deploy models.
- [ ] Implement CI/CD.
- [ ] Implement MLOps.
- [ ] Implement LLMOps.
- [ ] Monitor production AI systems.
- [ ] Design for reliability, scalability, security, and cost.

## Oracle Cloud Infrastructure
- [ ] Navigate OCI confidently.
- [ ] Configure IAM correctly.
- [ ] Configure OCI networking.
- [ ] Use Object Storage.
- [ ] Use the OCI Python SDK.
- [ ] Build ML solutions in OCI Data Science.
- [ ] Deploy ML models in OCI.
- [ ] Use OCI Language.
- [ ] Use OCI Speech.
- [ ] Use OCI Vision.
- [ ] Use OCI Document Understanding.
- [ ] Use OCI Generative AI chat models.
- [ ] Use OCI embedding models.
- [ ] Use OCI reranking.
- [ ] Build OCI-based vector-search/RAG systems.
- [ ] Build OCI Enterprise AI Agents.
- [ ] Use function calling.
- [ ] Use file/vector retrieval tools.
- [ ] Use MCP-enabled tools where appropriate.
- [ ] Build NL2SQL-based solutions where appropriate.
- [ ] Apply OCI AI guardrails and governance.
- [ ] Build secure, monitored, production-grade AI systems on OCI.

## Course Completion
- [ ] Complete every required phase.
- [ ] Complete every required from-scratch implementation.
- [ ] Complete every phase project.
- [ ] Complete the OCI service projects.
- [ ] Complete the final production capstone.
- [ ] Perform the final OCI AI coverage audit.
- [ ] Be able to design an AI solution before choosing an AI service or framework.
- [ ] Be able to explain the underlying principles instead of relying solely on libraries.
- [ ] Be able to determine when classical software is preferable to ML.
- [ ] Be able to determine when classical ML is preferable to deep learning.
- [ ] Be able to determine when a conventional ML model is preferable to an LLM.
- [ ] Be able to determine when RAG is preferable to fine-tuning.
- [ ] Be able to determine when deterministic workflows are preferable to AI agents.
- [ ] Be able to take an AI problem from raw data → experiment → model → evaluation → deployment → monitoring on OCI.
