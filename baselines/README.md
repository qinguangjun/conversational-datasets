
```

export TFHUB_CACHE_DIR=/my_module_cache

DATADIR=gs://your-bucket/reddit/YYYYMMDD

python baselines/run_baseline.py  \
  --method BM25 \
  --train_dataset ${DATADIR?}/train-* \
  --test_dataset ${DATADIR?}/test-*

```