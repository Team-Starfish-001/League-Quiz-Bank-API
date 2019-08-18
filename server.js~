const express = require('express')
const bodyparser = require('body-parser')
const app = express()

app.use(bodyparser.json())
bodyparser.urlencoded({
	extended: true
}
)
app.get('/getQuiz', (req, res) => {
    res.send({
        "headers": [
          "Quiz Name",
          "Author",
          "Create Date",
          "Action"
        ],
        "rows": [
          [
            "Quiz 1",
            "John Smith",
            "10/25/18",
            "ACTION"
          ],
          [
            "Quiz 2",
            "John Smith",
            "10/32/18",
            "ACTION"
          ],
          [
            "Quiz 3",
            "John Smith",
            "11/7/18",
            "ACTION"
          ],
          [
            "Quiz 4",
            "John Smith",
            "11/7/18",
            "ACTION"
          ]
        ]
      });
})
app.post('/getQuiz', (req,res) => {
    console.log(req.body);
    res.send(req.body)
})

app.listen(8080, () => console.log("Server Started on Port 8080!!!"))