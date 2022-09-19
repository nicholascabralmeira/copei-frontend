<template>
    <section class="section">
        <div class="columns is-centered">
            <div class="column is-4">
                <form class="box">
                    <div class="field">
                        <label class="label">Nome Completo</label>
                        <div class="control">
                            <input class="input" type="email" placeholder="e.g. alex@example.com">
                        </div>
                    </div>


                    <b-field label="Grouped">
                        <b-select placeholder="Estado" icon="earth">

                            <option value="flint">Parana</option>
                            <option value="flint">Rio Grande do Sul</option>
                            <option value="flint">Sao Paulo</option>
                            <option value="flint">Manaus</option>
                            <option value="flint">Brasilia</option>
                            <option value="flint">Salvador</option>


                        </b-select>
                    
                    
                        <b-select placeholder="Cidade" icon="earth">

                            <option value="flint">Curitiba</option>
                            <option value="flint">Cascavel</option>
                            <option value="flint">Pato Branco</option>
                            <option value="flint">Marechal</option>

                        </b-select>

                    </b-field>

                    <div class="field">
                        <label class="label">Username</label>
                        <div class="control has-icons-left has-icons-right">
                            <input class="input is-success" type="text" placeholder="Text input" value="joaozinho34">
                            <span class="icon is-small is-left">
                                <i class="fas fa-user"></i>
                            </span>
                            <span class="icon is-small is-right">
                                <i class="fas fa-check"></i>
                            </span>
                        </div>
                        <p class="help is-success">This username is available</p>
                    </div>
                    <b-field label="Data de nascimento">
                        <b-datepicker v-model="selected" :show-week-number="showWeekNumber" :locale="locale"
                            placeholder="Click to select..." icon="calendar-today"
                            :icon-right="selected ? 'close-circle' : ''" icon-right-clickable
                            @icon-right-click="clearDate" trap-focus>
                        </b-datepicker>
                    </b-field>


                    <div class="field">
                        <label class="label">email</label>
                        <div class="control">
                            <input class="input" type="email" placeholder="e.g. alex@example.com">
                        </div>
                    </div>


                    <div class="field">
                        <label class="label">Senha</label>
                        <div class="control">
                            <input class="input" type="password" placeholder="********">
                        </div>
                    </div>

                    <div class="field">
                        <label class="label">Confirmar Senha</label>
                        <div class="control">
                            <input class="input" type="password" placeholder="********">
                        </div>
                    </div>



                    <button class="button is-primary">Entrar</button>
                </form>
            </div>
        </div>

    </section>


</template>