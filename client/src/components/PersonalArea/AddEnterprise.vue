<template>
    <div class="container" style="margin-top: 100px; margin-bottom: 100px">
        <h1><i class="fa fa-long-arrow-left" aria-hidden="true" style="font-size: 20px; margin-right: 10px; color: #149B5F"
        onclick="window.location.href='/personalArea/myEnterprises'"></i>Добавить предприятие</h1>
        <div class="add-enterprise">
            <div class="row">
        <div class="col-md-9">
        <h3>Основные данные</h3>
        <div class="row">
            <div class="col-sm-6">
            <label for="title" class="label">Заголовок*</label>
            <input id="title" type="text" class="input" v-model="title" placeholder="Введите название">
            </div>
            <div class="col-sm-6">
            <label for="activity" class="label">Вид деятельности</label>
                <select name="category" id="category" class="select1">
                    <option value="" disabled selected>Деятельность</option>
                    <option value="1">Volvo</option>
                </select>
            </div>
        </div>
        <h3>Контактная информация</h3>
        <div class="row">
            <div class="col-sm-6">
            <label for="surname" class="label">Фамилия*</label>
            <input id="surname" type="text" class="input" v-model="surname">
            <label for="name" class="label">Имя*</label>
            <input id="name" type="text" class="input" v-model="name">
            </div>
            <div class="col-sm-6">
            <label for="patronym" class="label">Отчество*</label>
            <input id="patronym" type="text" class="input" v-model="patronym">
            <label for="phone" class="label">Номер телефона*</label>
            <input id="phone" type="tel" class="input" v-model="phone">
            </div>
        </div>
        <h3>Фотографии</h3>
        <p>Перетащите фото сюда или выберите их на своем компьютере…</p>
        <div class="row" style="margin-left: 0px">
            <div class="col-sm-3 col-md-3 col-xs-3" id="picture">
            <i class="fa fa-camera" aria-hidden="true" id="camera"></i>
            <p>Добавить</p>
            </div>
        </div>
        <p style="color: #8D8D92; font-size: 10px">Первое фото будет отображаться в результатах поиска, выберите наиболее
            удачное. <br>
            Вы можете загрузить до 10 фотографий в формате JPG или PNG.<br>
            Максимальный размер фото — 15MB.</p>
        <hr id="horizontal-line">
        <div class="row">
            <div class="col-md-3">
            <h3 style="margin-bottom: 0px">Элеватор</h3>
            </div>
            <div class="col-md-6">
            <select name="category" id="category" class="select2" style="margin-bottom: 0px">
                <option value="" disabled selected>Выберите элеватор</option>
                <option value="1">Volvo</option>
            </select>
            </div>
            <div class="col-md-3">
            <a>Показать на карте</a>
            </div>
        </div>
        <hr id="horizontal-line">
        <h3>Населенный пункт</h3>
        <div class="row">
            <div class="col-md-6">
            <select name="category" id="category" class="select1">
                <option value="1">Volvo</option>
            </select>
            </div>
            <div class="col-md-6" style="text-align: right">
            <a>Вставить мои данные</a>
            </div>
        </div>
        <button type="button" class="btn btn-primary">Продолжить</button>
        </div>

        <div class="col-md-3" style="padding-left: 50px">
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Основные данные 
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Параметры 
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Цена 
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Фотографии
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Элеватор 
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Населенный пункт
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Вид деятельности 
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Описание
            </label>
            <label for="generalData" class="add-announcement-checkbox-label">
            <input class="add-announcement-checkbox" type="checkbox" value="generalData" id="generalData">Контактные данные 
            </label>
        </div>
      </div>
        </div>
    </div>
</template>

<style>

h1 {
  font-size: 30px;
  font-weight: bold;
}

.add-enterprise {
  margin-top: 50px;
  background-color: white;
  padding: 50px;
  border-radius: 0px 0px 5px 5px;
}

#add-announcement-container {
  margin-top: 100px;
  margin-bottom: 100px;
}

h3 {
  font-size: 20px;
  margin-bottom: 30px;
}

.row {
  margin-bottom: 20px;
}

#camera {
  font-size: 50px;
  color: #B8B8B8;
  margin-bottom: 10px;
}

.select1{
    border: 0px;
    border-bottom: 1px solid #8A8A8A;
    width: 100%;
    font-size: 14px;
    margin-bottom: 20px;
    outline: 0px;
    background-color: white;
}


.select2{
    border: 0px;
    width: 100%;
    font-size: 14px;
    margin-bottom: 20px;
}

.label {
  font-size: 12px;
  line-height: 20px;
  color: #A9A9A9;
  text-align: start;
}

.add-announcement-checkbox{
    margin-right: 10px;
}

.add-announcement-checkbox-label{
    font-size: 14px;
}

label,
.input {
  color: #000000;
  display: block;
  border: .2px;
  font-size: 14px;
}

.input:focus {
  border-bottom: 1px solid #149B5F;
}

#horizontal-line {
  color: #E1E8EE;
  height: 1px;
}

.input {
  border-bottom: 1px solid #8A8A8A;
  outline: none;
  margin-bottom: 20px;
  width: 100%;
}

#picture {
  background-color: #F4F4F4;
  height: 160px;
  color: #7A7A7A;
  font-size: 10px;
  margin-right: 0px;
  text-align: center;
  padding-top: 50px;
}

</style>