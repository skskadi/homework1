# homework1

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>简历</title>
  </head>
  <body>
    <table border="1" width="600">
      <caption>
        基本信息
      </caption>
      <tr>
        <th>姓名</th><td>熊云政</td><th>性别</th><td>男</td><th>出生日期</th>
        <td>2004/11/13</td>
        <td rowspan="5">
          <img src="images/img_avatar.png"alt="错误"width="150"height="150"/>
        </td>
      </tr>
      <tr>
        <th>政治面貌</th><td>群众</td><th>籍贯</th><td>湖北咸宁</td>                    <th>民族</th><td>汉族</td>
      </tr>
      <tr>
        <th>婚姻状况</th><td>未婚</td><th>学历</th>
        <td>本科</td><th>专业</th><td>软件工程</td>
      </tr>
      <tr>
        <th>联系电话</th><td colspan="2">15342662700</td>
        <th>邮箱</th><td colspan="3">2326048385@qq.com</td>
      </tr>
      <tr>
        <th>身份证号</th><td colspan="2">33333333333333</td>
        <th>通讯地址</th><td colspan="3">安徽省合肥市宿松路</td>
      </tr>
      <tr>
        <th rowspan="2">相关证书</th><td colspan="2">获取时间</td>
        <td colspan="3">证书名称</td><td>发放单位</td>
      </tr>
      <tr>
        <td colspan="2">&nbsp</td><td colspan="3">&nbsp</td>
        <td colspan="2">&nbsp</td>
      </tr>
    </table>
  </body>
</html>




<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>注册页面</title>
  </head>
  <body>
    <div>
      <h4 span style="color: rgb(0, 21, 255)">欢迎注册会员</h4>
    </div>
    <form>
      手机号码：
      <input type="text" placeholder="11位手机号" />
      <span style="color: rgb(255, 0, 0)">必填</span>
      <br />
      创建密码：
      <input type="password" maxlength="8" placeholder="8位密码" />
      <span style="color: rgb(255, 0, 0)">必填</span>
      <br />
      注册邮箱：
      <input type="text" placeholder="例如wustzz@sina.com" />
      <span style="color: rgb(255, 0, 0)">必填</span>
      <br />
      验证码： <input type="text" /><br />
      性别：<input type="radio" name="sex" value="male" checked="checked" /> 男<input type="radio" name="sex" value="female" /> 女<br />
      生日：
      <input type="text" placeholder="年/月/日" />
      <br />
      年龄：
      <input type="text" />
      <br />
      籍贯：
      <select name="major">
        <option value="0">湖北</option>
      </select>
      <select>
        <option value="0">武汉</option>
      </select>
      <br />
      个人学历：
      <select>
        <option value="0">本科</option>
        <option value="1" selected="selected">专科</option>
      </select>
      <br />
      月薪
      <input type="range" id="score"name="score"min="2500"max="15000"step="1" value="5000"/>
      <span id="msg"
        ><script>
          var msg = document.getElementById("msg");
          window.onload = function () {
            msg.innerHTML = document.getElementById("score").value;
          };
          document.getElementById("score").onchange = function () {
            msg.innerHTML = this.value;
          };
        </script></span
      >
      <br />
      个人爱好：
      <label>
        <input type="checkbox" name="like" value="football" />唱歌
      </label>
      <label>
        <input type="checkbox" name="like" value="basketball" />跑步
      </label>
      <label>
        <input type="checkbox" name="like" value="football" />游泳
      </label> 
      <br>
      个人照片：<input type="file" name="myfile" accept="文件类型">
      <br>
      个人简介：<br>
<textarea name="intro" cols="50" rows="10"></textarea>
<br>
<input type="submit" value="提交">
<input type="reset" value="重填">
    </form>
  </body>
</html>
