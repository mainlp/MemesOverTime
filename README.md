# MemesOverTime


# MemesOverTime Dataset Files

## 1. `reddit_post_meta.csv`
Reddit post-level metadata sourced directly from the Reddit data dump.

| Column | Type | Description |
|--------|------|-------------|
| `post_id` | str | Unique Reddit post ID |
| `YYYY-MM` | str | Post date in `YYYY-MM` format |
| `image_url` | str | Original Reddit image URL |
| `subreddit` | str | Subreddit name |
| `subreddit_id` | str | Subreddit ID (e.g. `t5_xxxxx`) |
| `upvotes` | int | Post score (upvotes) |

## 2. `template_annotation.csv`
Template-level annotations mapping each post to its meme template hierarchy.

| Column | Type | Description |
|--------|------|-------------|
| `post_id` | str | Unique Reddit post ID |
| `template_id` | int | Top-level meme template ID |
| `cluster_id` | int | Visual cluster ID |
| `subcluster_local_id` | int | Local subcluster ID within the cluster |
