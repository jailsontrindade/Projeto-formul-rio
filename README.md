<!DOCTYPE html>
<html>
    <head>
        <title>Cadastro de veículos</title>
        <meta chasert="utf-8">
        <link rel="stylesheet" type="text/css" href="css/styles.css"/>
    </head>
    <bory>
        <div class="container">
            <div class="header">
                <h3>Cadastre seu veículo para vender mais rápido!</h3>
            </div>
            <div class="form-container">
                <div class="form-header">
                    <p>Cadastro</p>
                </div>
                <div class="form-bory">
                    <h1 class="form-title">Venda fácil seu veículo!</h1>
                    <p>Descreva as características do seu veículo e marque todos os opcionais e 
                    características que ele possui </p>
                    <form>
                  <div class="box-input">
                            <label for="title">
                                Título do anúncio:
                                <span class="required-field">*</span>
                            </label>
                            <input type="text" name="title" id="title" class="block"
                                placeholder="Defina um título para seu veículo"
                                minlength="1" maxlength="30" required>
                            </div> 
                        </div>      
                        <div class="box-input">
                            <label for="price">Preço do veículo:
                                <span class="required-field">*</span></label>
                            <input type="number" id="price" name="price" class="block" required>
                        </div>
                        <div class="box-input">
                            <label for="description">Descrição:
                                <span class="required-field">*</span> 
                            </label>
                            <textarea 
                            id="description" 
                            name="descripton" 
                            class="block"
                            cols="30"
                            rows="10"
                            required
                            placeholder="Descreva seu veículo"
                            >
                            </textarea>
                        </div>
                        <div class="box-input">
                            <label for="unique_owner">único dono?
                                <span class="required-field">*</span>
                            </label>
                            <select id="unique_owner" name="unique_owner" required>
                                <option value="">Selecione...</option>
                                <option value="1">Sim</option>
                                <option value="0">Não</option>

                            </select>
                        </div>
                       <div class="box-input">
                            <label for="brand">
                                Marca:
                                <span class="required-field">*</span>
                            </label>
                            <input type="text" name="brand" id="brand" class="block"
                                placeholder="Digite a marca do seu veículo" required>
                        </div>
                        <div class="box-input">
                            <label for="model">
                                Modelo:
                                <span class="required-field">*</span>
                            </label>
                            <input type="text" name="model" id="model" class="block"
                                placeholder="Digite o Modelo do seu veículo" required>
                        </div>
                        <div class="box-input">
                            <label for="mileage">
                                Kilometragem:
                                <span class="required-field">*</span>
                            </label>
                            <input type="number" name="mileage" id="mileage" class="block" required>
                        </div>
                        <div class="box-input">
                            <label for="purchase_date">
                                Data da compra do veículo:
                                <span class="required-field">*</span>
                            </label>
                            <input 
                            type="date" 
                            name="purchase_date" 
                            id="purchase_date" 
                            class="block" 
                            required
                        >
                        </div>
                        <div class="box-input">
                            <p>Câmbio: <span class="required-field">*</span></p>
                            <input type="radio" id="manual" name="gear">
                            <label for="manual">Manual</label>
                            <input type="radio" id="auto" name="gear">
                            <label for="auto">Automático</label>
                        </div>
                        <div class="optional_box">
                            <p>Opcionais:</p>
                            <ul class="optional_list">
                                <li>
                                    <input type="checkbox" id="airbag" name="optional[]" value="
                                    airbag">
                                    <label for="airbag">Airbag</label>
                                </li>
                                <li>
                                    <input type="checkbox" id="alarme" name="optional[]" value="
                                    alarme">
                                    <label for="alarme">Alarme</label>
                                </li>
                                <li>
                                    <input type="checkbox" id="ac" name="optional[]" value="
                                    ac">
                                    <label for="ac">Ar Condicionado</label>
                                </li>
                                <li>
                                    <input type="checkbox" id="eletric_lock" name="optional[]" value="
                                    eletric_lock">
                                    <label for="eletric_lock">Trava Elétrica</label>
                                </li> 
                            </ul>
                        </div>
                        <div class="optional-box">
                            <ul class="optional_list">
                                <li>
                                    <input type="checkbox" id="eletric_window" name="optional[]" value="eletric_window">
                                    <label for="eletric_window">Vidro Elétrico</label>
                                </li>
                                <li>
                                    <input type="checkbox" id="speakers" name="optional[]" value="
                                    speakers">
                                    <label for="speakers">Som</label>
                                </li>
                                <li>
                                    <input type="checkbox" id="reverse_camera" name="optional[]" value="
                                    reverse_camera">
                                    <label for="reverse_camera">Câmera de Ré</label>
                                </li>
                                <li>
                                    <input type="checkbox" id="leather_seat" name="optional[]" value="
                                    leather_seat">
                                    <label for="leather_seat">Banco de Couro</label>
                                </li> 
                            </ul>
                        </div>
                        <div clas="box-input">
                            <p>Envie imagens do veículo: <span class="required-field">*</span></p>
                            <input 
                            type="file" 
                            multiple accept="image/png,image/jpg" 
                            id="images"
                            required
                            >
                        </div>
                        <input type="submit" class="btn-submit" value="Cadastrar">    
                    </form>
                </div>
            </div>
        </div>
    </bory>
</html>

_______________________________________________________________________________________________________________________________________________________________

/*reset*/
bory {
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
    background-color: #673AB7;
}

html{background-color: #d3d3d3;}


h1,h2,h3,h4,h5 {
    color:#333;
}

p,label {
    color:#444;
}

input {
    border: 1px solid transparent;
    border-bottom: 1px solid #CCC;
    padding: 10px 0px;

}

input [type=text], input[type=number], input[type=date], input[type=file] {
    width: 400px;
} 
.block{width:50%;}
textarea {
    padding: 10px 5px;
    width: 400px;
}

/* cabecalho da pagina*/
.header {
    height: 160px;
    padding: 20px;
    background-color: #673AB7;
}

.header h3 {
    color: #FFF;
    margin-top: 0;
}

/*corpo formulario*/

.form-bory {
    padding: 30px;
}

.form-title {
    margin: 0;
}

.required-field {
    color: #D80835;
}

.box-input {
    margin-bottom: 30px;
}

.block {
    display: block;
} 

.optional_box {
    display: inline-block;
    margin-right: 30px;
}

.option_list {
    padding-left: 0;
}

.optional_list li {
    list-style: none;
}

/*container do formulario*/
.form-container {
    background-color: #FFF;
    width: 60%;
    margin-left: auto;
    margin-right: auto;
    position: relative;
    top: -62px;
}

/*cabecalho do formulario*/
.form-header {
    border-bottom: 1px solid #DFDFDF;
    height: 45px;
}

.form-header p {
    color: #673AB7;
    border-bottom: 2px solid #673AB7;
    width: 100px;
    text-align: center;
    margin-right: auto;
    margin-left: auto;
    text-transform: uppercase;
    height: 45px;
    line-height: 45px;
}

.btn-submit {
    background-color: #673AB7;
    color: #FFF;
    border: 2px solid transparent;
    width: 150px;
    height: 50px;
    text-transform: uppercase;
    cursor: pointer;
    transition: .5s;
}

.btn-submit:hover {
    background-color: #FFF;
    border-color: #673AB7;
    color: #673AB7;
}
