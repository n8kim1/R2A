python src/main.py --mode=train_r2a  --num_classes=2,2  --src_dataset=beer0 --tar_dataset=hotel --save --epoch_size=8 --hidden_dim=25 --rnn_size=100
first batch of saved runs
model saved
**FOR LATER (GOLD ATTN) MAKE SURE TO DUPE THE MODEL**

python src/main.py --mode=test_r2a  --num_classes=2,2  --src_dataset=beer0 --tar_dataset=hotel_Cleanliness  --snapshot=saved-runs/train_r2a/beer0_hotel_16703874504035458/best --test_path=../data/target/hotel_Cleanliness.train --batch_size=1
try to predict attention
normalized etc so yay


python src/main.py --mode=test_clf  --num_classes=2  --src_dataset=hotel_Cleanliness  --snapshot=saved-runs/train_r2a/beer0_hotel_16703874504035458/best --test_path=../data/target/hotel_Cleanliness.train --batch_size=1 --hidden_dim=25 --rnn_size=100
get gold attn (from building a standard oracle classifier)