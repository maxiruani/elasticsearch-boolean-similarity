
# Elasticsearch Boolean Similarity Plugin

Simple similarity that gives terms a score that is equal to their query boost. This similarity is typically used with disabled norms since neither document statistics nor index statistics are used for scoring. That said, if norms are enabled, they will be computed the same way as SimilarityBase and BM25Similarity with SimilarityBase#setDiscountOverlaps(boolean) discounted overlaps so that the {@link Similarity} can be changed after the index has been created.

## Build

mvn clean package

## Install

Run ./scripts/install-plugin.sh

Re-start elasticsearch

## Examples

Run ./examples/example.sh
