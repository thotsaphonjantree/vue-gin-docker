FROM golang:latest

WORKDIR /app

COPY . .

RUN go get "github.com/jinzhu/gorm"

RUN go get "github.com/go-sql-driver/mysql"

RUN go get "github.com/gin-gonic/gin"

RUN go get "github.com/gin-contrib/cors"

RUN go build -o goserver .

CMD ["./goserver"]

