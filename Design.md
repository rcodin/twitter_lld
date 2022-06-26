post tweets
follow/unfollow users
view 10 most recent tweets in users news feed


1) uid to identify the users
2) we can store tweets with timestamp
3) we can maintain a follower list. But, to unfollow someone is expensive here. we can use a unordered_set for it.
4) to get feed we go through the follower list and maintain top 10 followers. We can use a min heap based algorithm. It maintains top 10 tweets as we go through. At each tweet we compare min time stamp with existing timestamp. If it's small than pop the min and push current tweet
