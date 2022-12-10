
## Bộ dữ liệu 
#### Nguồn dữ liệu
  https://finance.yahoo.com/quote/AMZN/history?period1=1226102400&period2=1670457600&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true

#### Mô tả dữ liệu
  Mỗi bộ gồm hai tập dữ liệu là tập train và tập test nhãn mỗi đầu dòng là nhãn tương ứng với bộ dữ liệu liền sau nó
## Code 

Sử dụng ngôn ngữ python, môi trường chạy google colab

## Kết quả
Có hai bảng thống kê bảng thứ nhất là lấy ra lần mà có giá trị hàm loss nhỏ nhất, bảng thứ hai lấy ra giá trị accuracy lớn nhất
#### Bảng 1
| Bộ dữ liệu | Thuật toán |loss | accuracy| val_loss |val_accuracy|lr|
|--------------|-------|------|-------|---------|---------|-----------|
| 9class_3day |MLP |2.08299518 | 0.233486950 |2.94052839| 0.289320379|0.00100000005|
|             |FCN|0.00865046028| 0.996927798|10.5463867  |0.669902921|0.0000999999975|
|             | Resnet |[3.18383500e-02|  9.92319524e-01| 2.18130589e+00| 7.30097115e-01|9.99999975e-05|
|27 class_4day|MLP|3.08253288| 0.0988764018| 6.40033484| 0.0634920672|0.00100000005|
|             |FCN|[0.000679740100| 1.00000000| 20.8912544| 0.321995467|0.0000999999975|
|             |Resnet|
|81 class_5day|MLP|3.89044261| 0.0777777806| 17.6925926| 0.0431034490|0.00100000005|
|             |FCN|0.000811654900|1.00000000|63.6605606| 0.132183909|0.0000999999975|

|             |Resnet|
#### Bảng 2
## Tài liệu tham khảo

https://finance.yahoo.com/quote/AMZN/history?period1=1226102400&period2=1670457600&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true

@article{IsmailFawaz2018deep,
  Title                    = {Deep learning for time series classification: a review},
  Author                   = {Ismail Fawaz, Hassan and Forestier, Germain and Weber, Jonathan and Idoumghar, Lhassane and Muller, Pierre-Alain},
  journal                  = {Data Mining and Knowledge Discovery},
  Year                     = {2019},
  volume                   = {33},
  number                   = {4},
  pages                    = {917--963},
}

