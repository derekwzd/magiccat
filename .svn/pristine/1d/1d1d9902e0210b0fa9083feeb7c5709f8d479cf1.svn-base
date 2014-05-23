/* GET home page. */
exports.index = function(req, res){
  res.render('index', { title: 'Express' });
};

exports.about = function(req, res){
	res.render('about', {title: "Express"});
}

exports.gallary = function(req, res){
	res.render('gallary');
}

exports.test = function(req, res){
    res.render('test');
}


exports.img = function(req, res){
    res.render('img', {img: req.query.img});
}

exports.todo = function(req, res){
    res.render('todo');
}

exports.uploadImg = function(req, res){
    var fs = require("fs");
    console.log("文件默认属性："+req.files.uploadImg);  
    //console.log('原路径：'+ req.files.uploadImg.path);
        var obj = req.files.uploadImg;  
        var tmp_path = obj.path;  
        var new_path = "./public/uploads/"+obj.name;  
        //new_path = tmp_path;
        console.log("原路径："+ tmp_path); 
        console.log("现路径："+ new_path); 
        fs.rename(tmp_path,new_path,function(err){  
            if(err){
                throw err;
            }  
        })
        
    res.send('Post Over');
}