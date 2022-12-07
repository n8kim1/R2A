FAIL: don't use hotel dataset as src, 
cuz the dataloaders
python src/main.py --mode=train_r2a  --num_classes=2,2  --src_dataset=hotel --tar_dataset=hotel --save
resulted in tmp-runs/16703803420834692
simply train r2a using (only) the hotel dataset
is num_classes supposed to be 2? there's no true class label attached oddly

python src/main.py --mode=train_r2a  --num_classes=2,2  --src_dataset=beer0 --tar_dataset=hotel --save --epoch_size=8 --hidden_dim=25 --rnn_size=100
first batch of saved runs
model saved
